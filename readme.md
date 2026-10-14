# Allen Key (Hex Key)

## What it is?
An Allen key, also called a hex key, is an L-shaped hand tool used to turn screws and bolts that have a hexagonal socket in the head. The short leg gives a firm grip in tight spaces, and the long leg gives leverage.

## How it works?
The six flat faces of the key press against the six flat faces of the socket, so the turning force is spread evenly and the key is less likely to slip. The long leg acts as a lever, so a longer leg gives more torque for the same hand force.

## Size:
The size is the distance across opposite flats of the hexagon. Common metric sizes are 2, 2.5, 3, 4, 5, 6, 8 and 10 mm.

## Material:
Usually chrome vanadium or alloy steel, hardened for strength, with a coating such as black oxide or chrome to prevent rust.

## Uses:
Furniture assembly, bicycles, machinery and 3D printers.

## Advantages and limitations:
- Advantages: small, cheap, and works well in tight spaces.
- Limitations: it can round off the socket if the size is wrong or worn, and a standard key cannot be used at an angle.

## Conclusion
The Allen key is a simple tool that transfers torque efficiently through its hexagonal shape and L-bend.
![Allen key model](images/allen.png)
# Spur Gear Design Report

## 1. Introduction

Spur gears are mechanical components used to transmit rotational motion and power between **parallel shafts**. They have straight teeth and are commonly used in gearboxes, machine tools, and industrial machinery.

## 2. Objective

- To understand the working principle of spur gears.
- To study the important parameters involved in gear design.
- To understand gear strength and durability.

## 3. Working Principle

Spur gears transmit motion through the meshing of their teeth. When the driving gear rotates, it causes the driven gear to rotate in the **opposite direction**. The gear ratio depends on the number of teeth on each gear.

## 4. Important Parameters

| Parameter | Symbol | Description |
|---|---|---|
| Number of teeth | Z | Total number of teeth on the gear |
| Module | m | Ratio of pitch circle diameter to the number of teeth |
| Pitch circle diameter | d | Reference diameter used in gear design |
| Pressure angle | α | Determines the direction of force between meshing teeth |
| Face width | b | Width of the gear teeth along the shaft axis |

The module is calculated as:

$$
m = \frac{d}{Z}
$$

## 5. Design Specifications

| Item | Value |
|---|---|
| Gear ratio | 2 : 1 |
| Input gear (pinion) teeth, Z₁ | 20 |
| Output gear teeth, Z₂ | 40 |
| Module, m | 3 mm |
| Pressure angle, α | 20° |
| Material | Steel |

## 6. Design Calculations

**Gear ratio**

$$
i = \frac{Z_2}{Z_1} = \frac{40}{20} = 2
$$

**Pitch circle diameter** ($d = mZ$)

- Pinion: $d_1 = 3 \times 20 = 60$ mm
- Gear: $d_2 = 3 \times 40 = 120$ mm

**Centre distance**

$$
a = \frac{d_1 + d_2}{2} = \frac{60 + 120}{2} = 90 \text{ mm}
$$

**Other tooth dimensions** (standard full-depth 20° system)

| Quantity | Formula | Pinion | Gear |
|---|---|---|---|
| Addendum | $h_a = m$ | 3 mm | 3 mm |
| Dedendum | $h_f = 1.25m$ | 3.75 mm | 3.75 mm |
| Whole depth | $h = 2.25m$ | 6.75 mm | 6.75 mm |
| Outside diameter | $d_a = m(Z+2)$ | 66 mm | 126 mm |
| Root diameter | $d_f = m(Z-2.5)$ | 52.5 mm | 112.5 mm |
| Base circle diameter | $d_b = d\cos\alpha$ | 56.38 mm | 112.76 mm |
| Circular pitch | $p = \pi m$ | 9.42 mm | 9.42 mm |

**Speed relation**

$$
N_2 = \frac{N_1}{i} = \frac{N_1}{2}
$$

The output gear turns at half the input speed and, ignoring losses, delivers twice the input torque.

## 7. Gear Strength and Durability

A gear must resist two main kinds of failure:

- **Bending failure:** the tooth breaks at the root. Checked with the Lewis equation:

$$
\sigma_b = \frac{F_t}{b \, m \, Y}
$$

  where $F_t = \dfrac{2T}{d}$ is the tangential force and $Y$ is the Lewis form factor.

- **Surface (contact) failure:** pitting and wear on the tooth flanks from repeated contact stress.

Ways to improve strength and durability:

- Choose a strong material such as alloy steel and apply heat treatment or case hardening
- Use an adequate module and face width
- Provide proper lubrication and keep the lubricant clean
- Maintain accurate alignment and correct centre distance

## 8. Conclusion

Spur gears are simple, efficient, and widely used for power transmission between parallel shafts. For the designed pair (Z₁ = 20, Z₂ = 40, m = 3 mm, α = 20°), the gear ratio is 2:1 with a centre distance of 90 mm. Correct selection of module, tooth count, material, and lubrication ensures good strength and a long service life.
