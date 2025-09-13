# Pcileech-DNA-LOCK

Overview

DNALock is an open-source project that demonstrates a robust method for protecting FPGA-based DMA firmware through DNA ID validation.
Unlike common approaches that only block the FT601 channel, DNALock ensures that when DNA validation fails, the PCIe interface itself will not initialize.

This guarantees that no PCIe traffic can be captured, preventing memory or configuration space from being dumped by any means.

⚡ Key Features

Beyond FT601 Blocking

Existing methods only disable FT601, leaving PCIe activity exposed.

DNALock closes this gap completely.

PCIe Hard Lock

If the DNA ID is invalid, the PCIe channel will not enumerate at all.

Prevents any PCIe scanning or dumping attempts.

Source Code Included

Fully open-source implementation for research and integration.

Purpose

This release is intended for:

Developers seeking to integrate stronger DNA-based protection into FPGA DMA firmware.

Researchers studying secure PCIe device initialization.

For research and learning purposes only — not intended for misuse.

👉 More open-source projects will be released gradually.

💬 Join our Discord https://discord.gg/ajXCy3naaR to explore further and connect with the team.
