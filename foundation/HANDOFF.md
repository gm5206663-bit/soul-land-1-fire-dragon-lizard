# HANDOFF — how to work on this serial

Read this before you touch anything. Then `STATUS.md`.

## State in one breath

Chapter 1 shipped (`Chapter_01`, gated, 2902 words). All 13 lanes ruled.
Chapter 2 waits for the author's word — then: coverage file first, prose
second, gate third, STATUS same turn, push.

## The rules

1. **The author decides.** When he rules, quote him exactly, record it the
   same turn, run the gates, push. Never soften or invent a ruling.
2. **Never invent the OC's name.** Or any kid canon hasn't named.
3. **No System.** Not prose, not panels, not jokes.
4. **No fixed future.** Nothing in any file may pin his ceiling or
   endpoint.
5. **Canon untouched.** The friend walks beside canon's beats, never
   over them.
6. **Walls hold.** Never cross `SL1_GU_YUAN`, `soul_land_new`,
   `soul_land_holy_spirit`, or the SL4 fire-phoenix serial.
7. **The blank-sentence spine format is banned.** The author rejected it.
   Direction = canon road + natural consequences.
8. **Every chapter passes the gate** before it ships. Never weaken a
   gate to make it pass — fix the chapter.
9. **Contradiction rule:** found a conflict? Report it, cite both sources
   with dates, propose the smallest fix, and wait. Never silent-fix.
10. **Read order when you arrive:** `RULINGS_LOG` → `STATUS` →
    `OPEN_RULINGS` → this file's rules → the rest.

## Chapter process (every time)

1. Author says write.
2. Fetch the canon source; write `canon_coverage/Canon_Coverage_Chapter_NN.md`.
3. Write the chapter (plain, direct — his style: short paragraphs,
   real dialogue, concrete beats, a `## Footer` at the end).
4. `python3 tools/chapter_gate.py chapters/Chapter_NN.md` must PASS.
5. Update `STATUS.md` the same turn; append `SERIAL_LOG.md`.
6. Run `python3 tools/foundation_gate.py .` — must PASS.
7. Commit, push, present to the author.

## Authority order

The author's word → `RULINGS_LOG` → `STATUS` → this file →
`CANON_GROUND` receipts → other files → oldest files are history only.
