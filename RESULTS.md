# Lab 2 results — sealed core

Name:  Rares-Casian David
Student number:  91119545
Lab section:  L01
Core:  A — the letter on BRIEF.md
Machine:  Code Space 
Cores:  4 — an integer

## Tools and sources

Tools and sources: None

> Mandatory, even if it says "none". **No AI in the lab, at all** — see the
> README. Missing declaration: zero until you supply one. False one: misconduct.

## S2 — the defect · 40 marks

Three or more runs of `./bar given`, including one thread:

```
mode=given threads=1 rounds=2000 bad=0 firstbad=-1 checksum=ok correct=yes deadlock=no time=0.0017 cpu=0.0017
mode=given threads=1 rounds=2000 bad=0 firstbad=-1 checksum=ok correct=yes deadlock=no time=0.0016 cpu=0.0017
mode=given threads=1 rounds=2000 bad=0 firstbad=-1 checksum=ok correct=yes deadlock=no time=0.0017 cpu=0.0017
```

**S2.1** Name the mechanism: which claim in `given.c`'s header is false, and
what is actually happening? State the barrier's invariant and say which half of
it this code does not keep.



**S2.2** Prove it, in the form your `BRIEF.md` requires.

REPLACE THIS LINE

**S2.3** Minimality: what breaks if you do less, what it costs if you do more.

REPLACE THIS LINE

## S3 — the measurement · 30 marks

`./bar all <t> <rounds>` at 1, 2, 4 and 8 threads. Pasted, not retyped. If a
mode stops, `all` stops with it — run the modes one at a time and paste those.

```
```

| threads | given: correct? | given: time | given: cpu | fixed: time | fixed: cpu | alt: time | alt: cpu |
|---|---|---|---|---|---|---|---|
| 1 | | | | | | | |
| 2 | | | | | | | |
| 4 | | | | | | | |
| 8 | | | | | | | |

**S3.1** Reconcile with `PREDICTION.md`: quote what you predicted, say what
happened, account for the difference. If you were right, say what would have
made you wrong.

REPLACE THIS LINE

**S3.2** Which would you ship on this machine, **and what measurement would
change your mind?**

REPLACE THIS LINE

## S4 — explain-back · 15 marks

> Two or three sentences, your own words: someone who has not seen this code
> asks *what was wrong with it, and what did fixing it cost?*

REPLACE THIS LINE

## Anything you got stuck on

Optional. One or two lines.
