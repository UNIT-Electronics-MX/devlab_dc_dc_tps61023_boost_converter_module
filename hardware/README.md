# **Schematic**

<div align="center">
    <a href="resources/unit_sch_v_0_1_0_ue0087_tps61023_boost.pdf">
        <img src="resources/img/Schematics_icon.jpg?raw=false" width="500px"><br/> 
        Schematics (PDF)
    </a>
</div>



## Features

<div align="center">

| **Feature**                   | **Description**                                                                 |
|-------------------------------|---------------------------------------------------------------------------------|
| **Regulator IC**              | Texas Instruments TPS61023 – high-efficiency boost converter                   |
| **Input Voltage Range**       | 0.5 V to 5.5 V                                                                 |
| **Start-up Voltage**          | Operates from input as low as 0.7 V                                           |
| **Adjustable Output**         | Up to 5.5 V (via onboard multi-turn potentiometer)                            |
| **Output Current**            | Up to 1 A (depending on input/output conditions) *                              |
| **Efficiency**                | Up to 96 % under optimal conditions                                            |
| **Switching Frequency**       | ~2 MHz for reduced external component size                                    |
| **Protections**               | Overcurrent (OCP), thermal shutdown, undervoltage lockout (UVLO)              |
| **Form Factor**               | Breadboard-friendly 20.3 mm × 17.78 mm PCB                                         |
| **Applications**             | Ideal for LiPo boosts, USB power banks, solar panels, sensors, LEDs, prototyping |
| **Datasheet**                | [TPS61023 – Texas Instruments](https://www.ti.com/product/TPS61023)           |

</div>

*Output Current with Vout=5V:

<div align="center">

| **Vin** | **Iout (±10%)** |
|---------|-----------------|
| 2 V     | 300 mA          |
| 2.5 V   | 500 mA          |
| 3 V     | 800 mA          |
| 3.5 V   | 930 mA          |
| 4 V     | 1 A             |   

</div>

## Quick Start

1. **Wire up**  
   - Connect your lower-voltage source to **VIN +** and **VIN –**.  
   - Connect your load to **VOUT +** and **VOUT –** (common ground).  
2. **Adjust output**  
   - Use a small screwdriver to turn the potentiometer clockwise to raise voltage, counter-clockwise to lower.  
   - Monitor the output with a multimeter for precise setting.  
3. **Test under load**  
   - Apply a typical load and verify the voltage remains stable.



> **Tip:** Always start with the potentiometer turned fully counter-clockwise (lowest voltage) before applying power. Then slowly dial up to your target voltage while monitoring with a meter.



# **Pinout**

<div align="center">
    <a href="#">
        <img src="resources/unit_pinout_ue0087_tps61023_boost_v_1_0_0_en.jpg" width="450px"><br/> 
        Pinout Diagram
    </a>
</div>

---

## **Pin Descriptions**

<div align="center">

| **Pin Group**  | **Label**     | **Function**                                                               |
|----------------|---------------|----------------------------------------------------------------------------|
| **Input**      | VIN           | Positive input voltage. Connect your supply’s positive terminal here.     |
| **Input**      | GND Input     | Ground reference for input. Connect the supply’s negative terminal here.  |
| **Output**     | VOUT          | Boosted positive output. Provides regulated higher voltage.               |
| **Output**     | GND Output    | Output ground. Connect to your load's ground or system ground.            |
| **Adjustment** | POT           | Multi-turn potentiometer to set the output voltage precisely.             |

</div>

---

# **Board Topology**

<div align="center">
    <img src="resources/unit_topology_v_0_1_0_ue0087_tps61023_boost.png?raw=false" width="500px"><br/><br/>

| **Reference** | **Component**                 | **Description**                                     |
|---------------|-------------------------------|-----------------------------------------------------|
| **U1**        | TPS61023                      | Main boost converter IC by Texas Instruments        |
| **RV1**       | Potentiometer (multi-turn)    | Allows precise adjustment of the output voltage     |
| **L1**        | Power Indicator LED           | Lights up when input voltage is present             |
| **F1**        | Resettable Fuse (1 A)         | Protects the circuit from overcurrent conditions    |
| **JP1**       | VIN+ Pad                      | Positive terminal for power supply input            |
| **JP2**       | VIN– Pad                      | Ground terminal for power supply input              |
| **JP3**       | VOUT+ Pad                     | Positive terminal for boosted output                |
| **JP4**       | VOUT– Pad                     | Ground terminal for boosted output                  |

</div>

---

# **Dimensions**

<div align="center">
    <a href="#">
        <img src="resources/unit_dimension_v_0_1_0_ue0087_tps61023_boost.png" width="600px"><br/>
        Mechanical Dimensions
    </a>
</div>
