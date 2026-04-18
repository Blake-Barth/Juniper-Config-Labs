# Juniper-Config-Labs (EVE-NG)

A collection of high-level Juniper networking labs. This repository showcases functional configurations and topologies for **JNCIS**, **JNCIP**, and complex **Service Provider** projects, all built and validated in **EVE-NG**.

---

## 📂 Lab Collection

Each folder below contains a standalone project with all necessary assets for replication.

---

## 🛠 What's in Each Lab?

Every lab folder provides a comprehensive package for technical analysis and replication:

1.  **Topology Diagram:** A clear map of the network architecture (`./topology.png`).
2.  **Default/Base Configuration:** A `Default_Config.txt` file containing the initial setup applied to every node (system hostnames, root authentication, and management services) to ensure a consistent starting point.
3.  **Node-Specific Configurations:** Reference `.txt` files containing the validated logic for each specific node. These configurations were captured using the `show | display set` command to provide a clear, line-by-line template for your own implementation.
4.  **Lab README:** A breakdown of the technical objectives, protocols involved, and specific verification commands.

---

## 🚀 How to Use

1.  **Build:** Match your EVE-NG topology to the provided diagram.
2.  **Implementation:** * Open the baseline configuration file for a device (e.g., `R1.txt`).
    * On the EVE-NG console, enter configuration mode (`edit`).
    * **Audit the interface IDs:** Ensure the interfaces in the text file (e.g., `ge-0/0/0`) match the physical cabling in your EVE-NG lab.
    * Use the configuration text as a guide to apply the logic to your nodes.
3.  **Verification:** Check the included video or README to see the expected convergence results, then run the corresponding `show` commands on your own nodes to verify the state.

---

## 📝 Requirements

* **Platform:** EVE-NG (Community or Professional).
* **Images:** * **Routing:** vMX or vJunos-router images.
    * **Switching:** vQFX or **vJunos-EX** images.
