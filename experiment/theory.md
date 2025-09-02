
Bipolar Junction Transistors (**BJTs**) are **three-layer, two-junction** semiconductor devices — either **NPN** or **PNP** — that can **amplify** or **switch** electrical signals.  
They build directly on the physics of **PN junctions**, using **two back-to-back junctions** to control current flow.

**Regions of a BJT:**

- **Emitter (E):** Heavily doped to inject carriers efficiently.
- **Base (B):** Very thin and lightly doped to allow carriers to pass through with minimal recombination.
- **Collector (C):** Moderately doped and larger in area to collect carriers and dissipate heat.

<p><img src="images/bjt.png" ></p> 


---

## **3.2 Modes of Operation**

The operation of a BJT depends on the biasing of its two PN junctions:

- **Cut-off:** Both junctions reverse-biased → \( I_C \approx 0 \)
- **Active Mode:** Emitter-Base (**E-B**) forward biased, Collector-Base (**C-B**) reverse biased → transistor acts as an **amplifier**.
- **Saturation:** Both junctions forward-biased → \( I_C \) limited by the external circuit.
- **Reverse Active:** **E-B** reverse biased, **C-B** forward biased → reverse current gain \( \beta' \ll \beta \).

---

## **3.3 Carrier Transport in Active Mode**

In **active mode**, the forward bias on the **E-B** junction injects **majority carriers** from the **emitter** into the **base**.  
These carriers diffuse across the **thin base** and are swept into the **collector** by the reverse-biased **C-B junction’s electric field**.

**Transport Mechanisms:**

1. **Injection:** High emitter doping → large carrier injection into the base.
2. **Diffusion:** Carriers move through the base via **diffusion** due to a concentration gradient.
3. **Collection:** Carriers reaching the **base-collector** junction are quickly swept into the **collector**.

><p><img src="images/minority.png" ></p> 

---

## **3.4 Current Relationships**

The total emitter current:

$$
I_E = I_C + I_B
$$

The **common-base current gain** \( \alpha \):

$$
\alpha = \frac{I_C}{I_E}
$$

> For BJTs, \( 0.98 \leq \alpha < 1 \).

The **common-emitter current gain** \( \beta \):

$$
\beta = \frac{\alpha}{1 - \alpha}
$$

Thus, in active mode:

$$
I_C \approx \beta \, I_B
$$

---

## **3.5 Ebers–Moll Model**

The **Ebers–Moll model** describes a BJT in **all regions** of operation, using two coupled diodes.

**Collector Current Equation:**

$$
I_C = I_S \left( e^{V_{BE}/V_T} - 1 \right) - \alpha_R I_S \left( e^{V_{BC}/V_T} - 1 \right)
$$

**Emitter Current Equation:**

$$
I_E = \alpha_F I_S \left( e^{V_{BE}/V_T} - 1 \right) - I_S \left( e^{V_{BC}/V_T} - 1 \right)
$$

Where:

- \( I_S \) → Saturation current of the transistor  
- \( V_T \) → Thermal voltage (~25.85 mV at room temperature)  
- \( \alpha_F \) → Forward common-base gain  
- \( \alpha_R \) → Reverse common-base gain

<p><img src="images/Ebers.png" ></p> 

---

## **3.6 Output Characteristics**

In the **common-emitter configuration**, the **\( I_C \)–\( V_{CE} \)** characteristics in active mode are **nearly flat**, showing that:

- \( I_C \) is primarily controlled by **\( I_B \)**.
- A slight slope appears due to the **Early effect**.

<p><img src="images/ic.png" ></p> 

---

## **3.7 Summary of Key Equations**

**Collector current:**

$$
I_C = \beta I_B
$$

**Emitter current:**

$$
I_E = (\beta + 1) I_B
$$

**Active-mode equation:**

$$
I_C = I_S \left( e^{V_{BE}/V_T} - 1 \right)
$$

These equations are essential for designing **amplifiers** and **switching circuits** using BJTs.

---

