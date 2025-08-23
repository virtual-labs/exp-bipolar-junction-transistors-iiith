# 3. Bipolar Junction Transistors (BJT)

## 3.1 Topic Description

Bipolar Junction Transistors (BJTs) are three-layer, two-junction
semiconductor devices---either **NPN** or **PNP**---that can **amplify**
or **switch** electrical signals.\
They build directly on the physics of **PN junctions**, using two
back-to-back junctions to control current flow.

The three regions are:

-   **Emitter (E):** Heavily doped to inject carriers efficiently.
-   **Base (B):** Very thin and lightly doped to allow carriers to pass
    through with minimal recombination.
-   **Collector (C):** Moderately doped and larger in area to collect
    carriers and dissipate heat.

**\[Insert schematic diagram of NPN and PNP BJTs here\]**

------------------------------------------------------------------------

## 3.2 Modes of Operation

The operation of a BJT depends on the biasing of its two PN junctions:

-   **Cut-off:** Both junctions reverse-biased; collector current **IC ≈
    0**.
-   **Active Mode:** Emitter--Base (E-B) forward biased, Collector--Base
    (C-B) reverse biased; transistor acts as an **amplifier**.
-   **Saturation:** Both junctions forward-biased; **IC** limited by the
    external circuit.
-   **Reverse Active:** E-B reverse biased, C-B forward biased; reverse
    current gain **β′ ≪ β**.

**\[Insert energy band diagrams for each mode here\]**

------------------------------------------------------------------------

## 3.3 Carrier Transport in Active Mode

In active mode, the forward bias on the E-B junction injects majority
carriers from the **emitter** into the **base**.\
These carriers diffuse across the thin base and are swept into the
**collector** by the reverse-biased C-B junction's electric field.

Transport mechanisms:

1.  **Injection:** High emitter doping ensures a large number of
    carriers are injected into the base.
2.  **Diffusion Across Base:** Carriers move through the base by
    diffusion, due to the concentration gradient.
3.  **Collection:** Carriers reaching the base--collector junction are
    quickly swept into the collector.

**\[Insert graph of minority carrier distribution in base\]**

------------------------------------------------------------------------

## 3.4 Current Relationships

The key relationship between currents is:

``` math
I_E = I_C + I_B
```

The common-base current gain **α** is defined as:

``` math
α = I_C / I_E
```

with **0.98 ≤ α \< 1**.

The common-emitter current gain **β** is related to **α** by:

``` math
β = α / (1 − α)
```

Thus, in active mode:

``` math
I_C ≈ β I_B
```

------------------------------------------------------------------------

## 3.5 Ebers--Moll Model

The Ebers--Moll equations model the BJT in all regions of operation,
analogous to **two coupled diodes**.

For the **collector current**:

``` math
I_C = I_S (e^{V_{BE}/V_T} - 1) - α_R I_S (e^{V_{BC}/V_T} - 1)
```

For the **emitter current**:

``` math
I_E = α_F I_S (e^{V_{BE}/V_T} - 1) - I_S (e^{V_{BC}/V_T} - 1)
```

Where: - **I_S**: saturation current of the transistor - **V_T**:
thermal voltage (≈ 25.85 mV at room temperature) - **α_F**: forward
common-base gain - **α_R**: reverse common-base gain

**\[Insert schematic diagram of Ebers--Moll equivalent circuit here\]**

------------------------------------------------------------------------

## 3.6 Output Characteristics

In the **common-emitter** configuration, the **IC--VCE** characteristics
in active mode are nearly flat, indicating that **IC** is primarily
controlled by **IB** rather than **VCE**, except for a small slope due
to the **Early effect**.

**\[Insert IC--VCE family of curves here\]**

------------------------------------------------------------------------

## 3.7 Summary of Key Equations

``` math
I_C = β I_B
```

``` math
I_E = (β + 1) I_B
```

``` math
I_C = I_S (e^{V_{BE}/V_T} - 1)  \  \text{(Active mode)}
```

These relationships are essential for designing and analyzing amplifier
and switching circuits using BJTs.

------------------------------------------------------------------------

## 3.8 Suggested References

1.  R. F. Pierret, *Advanced Semiconductor Fundamentals*.
2.  S. M. Sze and K. Ng, *Physics of Semiconductor Devices*.
3.  B. G. Streetman and S. Banerjee, *Solid State Electronic Devices*.
