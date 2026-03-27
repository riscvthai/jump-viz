# jump-viz

**RISC-V JAL/JALR jump and control flow visualizer** — step through instruction sequences, watch the program counter move, see jump arcs animate in real time.

Live at: https://jumpviz.riscvthai.org/

\---

## What it does

An interactive step-through simulator showing how JAL, JALR, and their pseudoinstruction forms (j, jr, ret, call, tail) affect control flow. Animated jump arcs connect source and target instructions. The program counter advances one step at a time so the mechanics are visible.

Teaches: the difference between JAL (PC-relative) and JALR (register-indirect), how the link register works, how pseudoinstructions like `ret` and `call` expand, and what control flow actually looks like at the instruction level.

## How to run it

No install. No framework. No server required.

```sh
git clone https://github.com/riscvthai/jump-viz
cd jump-viz
# open index.html in any browser
```

Or visit the live demo at https://riscvthai.org/jump-viz/

## How to fork it

The instruction sequences are defined as JS arrays inside `index.html`. Add your own examples, translate the UI, adapt for your course.

## Files

```
index.html      ← complete visualizer, self-contained
README.md
```

## Author

Tran The Hao — Ho Chi Minh City University of Transport (UT-HCMC), Vietnam  
haott9953@ut.edu.vn

Built with assistance from Claude (Anthropic). Architecture analysis — MIPS to RISC-V
mapping, JAL/JALR differences, pseudoinstruction expansion — developed through a
collaborative Claude session: https://claude.ai/share/fe723119-0411-4f16-af55-2496d6ff5883

The author believes transparency about AI-assisted development is important,
especially in an educational context.

## History

* Mar 2026 — Initial MIPS JAL/JR version
* Mar 2026 — Adapted for RISC-V JAL/JALR, contributed to riscvthai.org

## License

MIT. Fork freely. Attribution appreciated.

## Related

* https://github.com/riscvthai/games — full suite index
* https://github.com/riscvthai/pseudobingo — pseudoinstruction bingo game
* https://riscvthai.org — Thai RISC-V educational resource
