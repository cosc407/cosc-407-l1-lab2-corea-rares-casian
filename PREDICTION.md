# Prediction sheet — push by 0:20, before you compile

> Marked on **having predicted** and on reconciling it in S3.1 — **not on being
> right.** A confident wrong prediction you then explain is full marks. A blank
> page is none. A page timestamped after your first run is worse than none.
>
> Read `src/given.c` and `BRIEF.md`. Run nothing.

Cores:  4 — from PREP.md
Lab 0 spread:  29.8 — the percentage, from PREP.md

> **P1.** `./bar given` on **one** thread — does it come out right? Yes/no, one
> sentence why.

No inside wait the count variable is never reset back to 0. this will cause count to not be equal to n after the first use of the barrier. 

> **P2.** On **8** threads, pick one and commit to it: right answer / wrong
> answer / it stops. If wrong, roughly how big is `bad`? If it stops, say at
> which of the two waits in a round.

wrong on 8 threads it will stop since the count is never reset. It will deadlock after the first wait. 

> **P3.** Three runs at 8 threads — **identical** numbers, or different? Think
> about this one before you write it; it is the most useful line on the page.

They will be identical since they will all deadlock after the first wait. since count is never reset back to 0 (assuming you dont create a new barrier each time and instead reuse the same one)

> **P4.** Seconds, before measuring. Orders of magnitude are what matter. `cpu`
> is process CPU time over all threads, so `cpu`/`time` is how many cores were
> busy — one number per box.

| | 1 thread: time | 8 threads: time | 8 threads: cpu/time |
|---|---|---|---|
| `given` | | | |
| `fixed` | | | |
| `alt` | | | |

> **P5.** Fastest and slowest at 8 threads? Name anything you expect to get
> **slower** as threads are added, and anything you expect to stop altogether.


slowest -> alt will deadlock and same with given 
fastest -> fixed since it will not deadlock


