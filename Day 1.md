# Day 1 Homework — Quadratics Studio: Structure, a Graded Answer, and a Pretzel

  

> This is **Day 1 of a 4-night project**. Each night you grow the *same* file. Save it as `Quadratics Studio.doenet` in your Doenet activities — you will reopen it tomorrow.

  

**Goal:** Stand up a clean, well-structured Doenet document with one auto-graded factoring question and a 6-problem factoring pretzel.

  

**New components this session:** `<section>`, `<title>`, `boxed`, `<aside>`, `includeAutoNumber`, `<p>`, `<em>`, `<alert>`, `<c>`, `<m>`, comments (`Cmd+/`), `<answer>`, `<award>`, `<mathInput>`, `credit`, `matchByExactPositions`, `caseInsensitiveMatch`, the pretzel template, `maxNumColumns`, `isDistractor`.

  

---

  

## Tasks

  

**1. Build the shell.**

- Create a new activity called **Quadratics Studio**.

- Add a top-level `<title>` and a **titled, `boxed` `<section>`**.

- Inside it, write a 2–3 sentence intro with `<p>`, using `<em>` and at least one `<alert>` for emphasis. Display a sample trinomial inline with `<m>` (e.g. `<m>x^2 + 5x + 6</m>`).

- Put the *student instructions* ("Factor each quadratic; enter your answer as a product of two binomials") inside an `<aside>` so they collapse.

- Add a comment header at the top (course / chapter / your name) using `Cmd+/`, mirroring the style in [Factoring Crossword (a=1).doenet](../../Polynomial%20Functions/Factoring%20Crossword%20(a=1).doenet).

  

**2. Add one auto-graded question.**

- Question: *Factor* `<m>x^2 + 5x + 6</m>`.

- Use the `answer` snippet (type `answer` in the editor and pick the snippet — it inserts a pre-structured template with a `<label>` included).

- Give a full-credit `<award>` for `(x+2)(x+3)` and a **partial-credit** `<award credit="0.5">` for a near-miss you choose (e.g. correct binomials, wrong signs).

- Order already doesn't matter for a product, so `(x+3)(x+2)` is accepted by default. If you ever need to *enforce* position, that attribute is `matchByExactPositions`; `caseInsensitiveMatch` is available for text answers.

- If the mathInput shows a red accessibility flag, give it a `<label>` for now. *(We make everything accessible on Day 4 — just clear this one flag today.)*

  

**3. Build a 6-problem factoring-trinomials pretzel.**

- Load the pretzel template from the code snippet (the 10-problem template shown in Session 1).

- **Delete problems down to 6.** Set `maxNumColumns="3"`.

- Fill each problem with a trinomial to factor and its answer. Keep numbers small and factorable (e.g. roots in 1–6).

- Mark **at least one** problem as a distractor with `isDistractor` (a trinomial that does *not* factor over the integers).

  

---

  

## Study first

- The Session 1 demo docs: the **broken-document fixer**, **Math Answer Examples** (in the scratchpad Load menu), and the **pretzel template** snippet.

- [Factoring Crossword (a=1).doenet](../../Polynomial%20Functions/Factoring%20Crossword%20(a=1).doenet) — for the comment header, `<aside>` instructions, and `<answer><award>` style.

- When stuck on a tag/attribute, use the **`?` help panel** → reference lookup rather than guessing.

  

## House conventions (apply every night)

- All answer computation goes in `<setup>` (you'll move things there tomorrow).

- **Grade precisely** — award full credit only to the intended factored form.

- Keep numbers **classroom-friendly**.

- Check [DOENETML_INTALG_REFERENCE.md](../../DOENETML_INTALG_REFERENCE.md) before inventing syntax.

  

## Done when

- [ ] The document renders with **no errors** (error panel clean).

- [ ] The factoring question grades a **right / wrong / partial** response correctly.

- [ ] `(x+2)(x+3)` **and** `(x+3)(x+2)` both earn full credit.

- [ ] The pretzel shows **6 problems in 3 columns** with at least one working **distractor**.

  

## Stretch (optional)

Add a second graded part asking for the **roots** of `x^2 + 5x + 6` (i.e. `x = -2, x = -3`) using a `mathList`.