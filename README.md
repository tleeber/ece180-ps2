# ECE180 Verilog Homework

# My Personal Notes
**Problem 1**
- I had never heard the term saturated used in this context, so I had to make sure it meant to leave the count at max.
- The _ni in rst_ni means that reset is active when low.
**Problem 2**




Two problems, building on the lab (`WORKBOOK.md`).

**Start here: [`HOMEWORK.md`](HOMEWORK.md)**

## Quick start

```bash
verilator --version     # need 5.0+;  apt-get install verilator  /  brew install verilator
make all                # run both problems
```

## Submission

Graded for **completion**.

1. Push this directory to a GitHub repo and submit the URL.
2. Run `make all`, screenshot the `P1 / P2` lines, upload to Gradescope.

Stuck on one? Submit anyway, and note in your README what you tried and where it broke.

## Layout

```
HOMEWORK.md    the assignment — read this
Makefile
rtl/           you edit these
tb/            testbenches — do not edit
```

## Problems

| | Topic | File |
|---|---|---|
| 1 | FSM: overlapping "1101" detector + saturating counter | `rtl/p1_seq_detect.sv` |
| 2 | Register file: dual combinational reads, sequential write, bypass | `rtl/p2_regfile.sv` |

## Targets

| | |
|---|---|
| `make pN` | run problem N |
| `make all` | run both |
| `make waveN` | run and dump `build/pN/pN.vcd` |
| `make clean` | |
