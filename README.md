![Asynchronous FIFO Banner](assets/Async_fifo.png)
# 🗂️ Asynchronous FIFO Design and Verification

## 📌 Project Overview

This repository contains the design and verification of an **Asynchronous FIFO (First-In-First-Out) memory** using Verilog.
The FIFO is designed to handle **two independent clock domains** (write clock and read clock) with proper synchronization to ensure safe data transfer.

---

## ⚙️ Features

* Parameterized FIFO size (depth & width)
* Independent Write and Read clock domains
* Reset logic implementation
* FIFO Full and Empty flag handling
* Support for simultaneous Read & Write across domains
* Pointer synchronization using 2-flop synchronizers

---

## 🧪 Test Cases Verified

The FIFO design has been validated against the following scenarios:

* Normal Write & Read operations
* FIFO Full condition
* FIFO Empty condition
* Write when FIFO is full
* Read when FIFO is empty
* Simultaneous Read & Write under asynchronous clocks
* Reset condition behavior
* Cross-domain pointer synchronization checks

---

## 📂 Repository Structure

```
├── async_fifo.v       # FIFO Design file  
├── async_fifo_tb.v    # Testbench file  
├── assets/            # Banner & Block diagram images  
│   ├── async_fifo_banner.png  
│   └── async_fifo_block.png  
└── README.md          # Project documentation  
```

## 📊 Sample Output

* FIFO operations with independent read & write clocks
* Flag status (Full / Empty)
* Test case validation logs from the testbench

---

## 🚀 Future Enhancements

* Synthesis validation on FPGA boards
* Error detection and correction support
* Coverage-driven verification with SystemVerilog/UVM

---

## 🤝 Contributions

Contributions are welcome! Feel free to fork this repo and submit pull requests.
