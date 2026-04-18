# Juniper-Config-Labs (EVE-NG)

A collection of high-level Juniper networking labs. This repository showcases functional configurations and topologies for **JNCIS**, **JNCIP**, and complex **Service Provider** projects, all built and validated in **EVE-NG**.

---

## 📂 Lab Collection

Each folder below contains a standalone project with the necessary configuration assets for replication.

> You can download official evaluation or licensed images directly from the [Juniper Networks Support Portal](https://support.juniper.net/support/downloads/).

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
2.  **Initial Setup:** * Access the EVE-NG console for each node.
    * Enter configuration mode (`edit`).
    * Apply the `Default_Config.txt` to establish consistent system settings and credentials.
3.  **Implementation:** * Open the node-specific configuration file (e.g., `R1.txt`).
    * **Audit the interface IDs:** Verify that the interfaces in the text file (e.g., `ge-0/0/0`) match your physical cabling in EVE-NG. 
    * Use the `show | display set` formatted text as a guide to apply the specific routing and switching logic to your nodes.
4.  **Verification:** Check the included video or README to see the expected convergence results, then run the corresponding `show` commands on your own nodes to verify the state. Check that full network connectivity exists using **Ping** and **Traceroute** to validate end-to-end reachability.

---

## 📝 Requirements

* **Platform:** EVE-NG (Community or Professional).
* **Images:** * **Routing:** vMX or vJunos-router images.
    * **Switching:** vQFX or **vJunos-EX** images.
