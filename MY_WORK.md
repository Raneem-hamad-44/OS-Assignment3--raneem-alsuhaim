# 📝 MY_WORK: Student Information, Development Log, Reflection & Answers

> This is the **only file** your instructor reads to grade Parts 3 and 4 (documentation and video). Everything you write here must be **in your own words**.

---

## 🛑 STOP: Read This Before You Do Anything Else

> ### 1️⃣ Read the whole `README.md` first
> The `README.md` in this repository contains the full instructions: how this assignment continues Assignment 1, the Chapter 5 recap, class descriptions, feature specifications, question prompts and the video script. **If you skip it, you will lose marks.**
>
> ### 2️⃣ Understand the full code before answering any question
> Open `SchedulerSimulationSync.java` and read it **from top to bottom**. You must be able to explain what `SharedStats`, `ReadyQueue`, `CpuWorker`, `RaceWindow.pause()`, `ReentrantLock` and `Semaphore` do **before** you write a single answer in Parts B and C. **Run the original starter first** (it is intentionally broken) and **save its output**: you need it for Question 1 of Part C.
>
> ### 3️⃣ Use only the code of this repository
> Work **only** on `SchedulerSimulationSync.java` from this repository. Do **not** copy or paste code from your previous assignments.
>
> ### 4️⃣ Commit many times, not once
> A single commit, or all commits made in the last hour, costs you **-0.5 mark**. See the [Commit Rules](#-commit-rules-mandatory) below.

**How to use this file:**
1. Fill in your **Student Information** (below) right now.
2. Follow the steps in the **Work Roadmap** in order.
3. Update the **Development Log** *every time* you work on the assignment, not at the end.
4. Do not delete any section header. Replace the `[...]` placeholders with your own text.

---

## 👤 Student Information

> ⚠️ **WARNING:** Fill this in first. Your name and ID must match the student ID you set in `SchedulerSimulationSync.java` (line 304) and the one you say in your video.

| Field | Your Answer |
|-------|-------------|
| **Full Name** | Raneem Hamad Alsuhaim |
| **Student ID** | 444051957 |
| **University Email** | 444051957@std.psau.edu.sa |
| **GitHub Username** | Raneem-hamad-44 |
| **Repository Link** | https://github.com/Raneem-hamad-44/OS-Assignment3--raneem-alsuhaim |
 
---

## 🎥 Video Link

**Video Link**: [Paste your video link here]

> ⚠️ **WARNING:** The video must be **publicly accessible** ("Anyone with the link can view") on **Google Drive**, **YouTube (Unlisted or Public)** or any other cloud file-sharing system. A private, restricted or broken link counts as a **missing video (-1 mark)**.
>
> 💡 **TIP:** Open the link in a **private/incognito window** before you submit. If it asks you to log in or request access, it is not public.
>
> 📌 **NOTE:** The link goes in **this file only** (`MY_WORK.md`), **not** in `README.md`. Name your video file `444051957_Assignment3_Demo.mp4`. It must last **2 to 3 minutes**.

---

## 🗺️ Work Roadmap (follow in this order)

| Step | What to do | Where | Marks |
|:----:|------------|-------|:-----:|
| 0 | Read `README.md`, read the full code, **run the original starter and save its output** (it fails on purpose) | Your IDE | – |
| 1 | Fork, rename, keep the repo **PUBLIC**, set your student ID (line 304), **commit** | GitHub + code | Part 1 (1) |
| 2 | Feature 1: Mutex lock on the ready queue, **commit** | Code | Part 2 (0.25) |
| 3 | Feature 2: Mutex lock(s) on the shared statistics, **commit** | Code | Part 2 (0.25) |
| 4 | Feature 3: Counting semaphore instead of busy waiting, **commit** | Code | Part 2 (0.5) |
| 5 | Development Log (5+ entries, different dates) | This file, Part A | Part 3 (0.5) |
| 6 | Reflection (4 questions) | This file, Part B | Part 3 (0.5) |
| 7 | Technical Answers (4 questions) | This file, Part C | Part 3 (0.5) |
| 8 | Record the video, upload it, paste the link above | Video + this file | Part 4 (1.5) |
| 9 | Final check, then submit the repo link on Blackboard | Blackboard | – |

> 💡 **TIP:** Tick each step off as you go. Do not leave the log, the reflection or the video for the last day.

---

## 🔁 Commit Rules (MANDATORY)

> ### ⚠️ MANY COMMITS ARE REQUIRED. A single bulk commit is penalized (-0.5 mark).

**Minimum: 4 meaningful commits. Aim for 7 or more.**

| # | Commit | Example message |
|:-:|--------|-----------------|
| 1 | Student ID set | `Set my student ID: 444051957` |
| 2 | Feature 1: Ready queue lock | `Feature 1: Protected the ready queue with a ReentrantLock` |
| 3 | Feature 2: Statistics locks | `Feature 2: Added locks to the shared statistics counters` |
| 4 | Feature 3: Semaphore | `Feature 3: Replaced busy waiting with a counting semaphore` |
| 5 | Development log entries | `Docs: Added development log entries` |
| 6 | Reflection and answers | `Docs: Completed reflection and technical answers` |
| 7 | Video link | `Docs: Added demo video link` |

**Rules:**
- ✅ **One commit per feature.** Do not put all three features in one commit.
- ✅ **Commit after each work session**, and after each part of this file.
- ✅ **Spread your commits over different dates.** Not all in one day.
- ❌ **Do not make all commits in the last hour** before the deadline (November 14, 2026).
- ❌ **No vague messages** like `done`, `update` or `final version`.

> 💡 **TIP:** Your commit history is checked and you **show it in your video** (at least 4 commits visible). Your development log dates should match your commit dates.
>
> 💡 **TIP:** **Use VS Code** (see *Recommended Development Environment* in `README.md` for the full setup). Sign in to GitHub in VS Code, then commit from the Source Control panel (Ctrl+Shift+G) → stage → write a message → Commit → Sync/Push. You can edit and commit this file the same way. **Pushing** matters: commits that are not pushed to GitHub are invisible to the instructor.

---

# Part A: Development Log (0.5 mark)

> ⚠️ **WARNING:** Minimum **5 entries**, spread over **different dates**. Five entries written on the same day, or written all at once at the end, will lose marks and look like a copy. Entry dates should be **between the start of the assignment and the deadline (November 14, 2026)**.

## Your Development Log

### Entry 1 - [November 3, 2026, 5:00 PM]
**What I did**: Forked the starter repository, configured my student ID, and executed the broken starter code

**Details**:
- Forked `makopt/OS-Assignment3-Starter-481` to my GitHub account (`Raneem-hamad-44`) and renamed it to `OS-Assignment3--raneem-alsuhaim`
- Updated `studentID` in `SchedulerSimulationSync.java` to `444051957`
- Ran the unmodified starter code to observe the concurrency bugs and saved the verification output
- Committed and pushed the student ID change (`Set my student ID: 444051957`)

**Challenges**: Seeing multiple CPUs pick the same process thread and crash with `IllegalThreadStateException` was confusing at first

**Solution**: Inspected `ReadyQueue.poll()` and saw that `RaceWindow.pause()` occurs right between `list.getFirst()` and `list.removeFirst()`, allowing two CPUs to grab the same head node

**Time spent**: 50 minutes

---

### Entry 2 - [November 5, 2026, 7:15 PM]
**What I did**: Implemented Feature 1 by protecting `ReadyQueue` with a `ReentrantLock`

**Details**:
- Imported `java.util.concurrent.locks.ReentrantLock` and declared `private final ReentrantLock queueLock = new ReentrantLock();` inside `ReadyQueue`
- Wrapped the bodies of `add()`, `poll()`, `processOf()`, and `snapshot()` in `queueLock.lock()` and `try / finally { queueLock.unlock(); }`
- Tested the simulation to confirm no duplicate thread starts or `IllegalThreadStateException` occurred
- Committed and pushed Feature 1 (`Feature 1: Protected the ready queue with a ReentrantLock`)

**Challenges**: Ensuring that every return path inside `poll()` (including when `list.isEmpty()` returns `null`) properly unlocks the mutex

**Solution**: Placed `queueLock.unlock()` inside a `finally` block so the lock is guaranteed to release regardless of how the method exits

**Time spent**: 45 minutes

---

### Entry 3 - [November 7, 2026, 6:00 PM]
**What I did**: Implemented Feature 2 by protecting `SharedStats` counters and getters with a `ReentrantLock`

**Details**:
- Declared `private static final ReentrantLock statsLock = new ReentrantLock();` in `SharedStats`
- Protected all three update methods (`incrementContextSwitch()`, `incrementCompletedProcess()`, and `addServiceTime()`) using `try / finally`
- Also protected the reader methods (`getCompletedProcessCount()`, `getContextSwitchCount()`, and `getTotalServiceTime()`) to prevent reading inconsistent mid-update values
- Committed and pushed Feature 2 (`Feature 2: Added locks to the shared statistics counters`)

**Challenges**: Deciding whether to use one lock for all three statistics or three separate locks per variable

**Solution**: Analyzed the short execution time of the arithmetic increments and decided on a single `statsLock` to keep the code clean, avoid extra lock overhead, and guarantee memory visibility across all getters

**Time spent**: 40 minutes

---

### Entry 4 - [November 9, 2026, 8:30 PM]
**What I did**: Implemented Feature 3 using a counting `Semaphore` to eliminate busy waiting

**Details**:
- Added `private final Semaphore availableProcesses = new Semaphore(0);` in `ReadyQueue`
- Called `availableProcesses.release()` at the end of `ReadyQueue.add()` after releasing `queueLock`
- Replaced the polling loop and `Thread.sleep(20)` in `CpuWorker.run()` with `readyQueue.waitForProcess()` (`acquire()`)
- Added `wakeAllCpus(SharedStats.totalCPUs)` when the final process completes so blocked CPU threads terminate cleanly
- Verified the program across 5 consecutive runs with all four checks showing `✔` and `Busy-waiting polls` at `0`
- Committed and pushed Feature 3 (`Feature 3: Replaced busy waiting with a counting semaphore`)

**Challenges**: During initial testing, the simulation hung at the very end because idle CPUs remained blocked on `acquire()` after the last process finished

**Solution**: Added a completion check after a process finishes its quantum so the CPU that completes the last process calls `availableProcesses.release(SharedStats.totalCPUs)` to wake all sleeping workers

**Time spent**: 1 hour 15 minutes

---

### Entry 5 - [November 11, 2026, 4:45 PM]
**What I did**: Documented the development log, reflection questions, and technical answers in `MY_WORK.md`

**Details**:
- Reviewed all sections of `README.md` and double-checked my starter vs. final verification outputs
- Filled in the student information table, development log entries, reflection answers, and technical answers in `MY_WORK.md`
- Committed and pushed the documentation updates

**Challenges**: Structuring clear step-by-step timelines for the race conditions observed in the starter output

**Solution**: Compared the expected values calculated from my seed (`444051957`) against the mismatched observed counts from my saved starter run

**Time spent**: 1 hour

---

## Development Log Summary

**Total time spent on assignment**: 4 hours 30 minutes

**Most challenging part**: Designing a clean shutdown mechanism for the `CpuWorker` threads in Feature 3 so they would not remain blocked indefinitely on `Semaphore.acquire()` after all processes finished.

**Most interesting learning**: Seeing how a tiny 1ms pause (`RaceWindow.pause()`) between reading and writing a shared variable reliably exposes lost updates and corrupted queue states that normally happen randomly in real operating systems.

**What I would do differently next time**: I would sketch out the semaphore permit lifecycle (initial permits, releases per enqueue, and final shutdown releases) on paper before writing the `CpuWorker` loop to avoid the initial termination hang.

---

# Part B: Reflection (0.5 mark)

## Question 1: What did you learn about synchronization?

**Your Answer:** *(5-7 sentences)*

Through this assignment, I learned how easily concurrent threads corrupt shared data when read-modify-write operations are not atomic. In the un-synchronized starter code, `RaceWindow.pause()` exposed how two CPUs could read the same value from `contextSwitchCount` or `ReadyQueue.list` before either thread wrote its update back. Using `ReentrantLock` with `try/finally` blocks taught me how mutual exclusion enforces that only one thread enters a critical section at a time while guaranteeing lock release even if an exception occurs. I also learned the difference between mutual exclusion locks and signaling mechanisms like a counting `Semaphore`, which coordinates producer-consumer execution without wasting CPU cycles. Seeing the verification block fail repeatedly before synchronization and pass consistently with `✔` after adding locks and a semaphore made these operating system concepts concrete.

## Question 2: What was the most challenging part of this assignment?

**Your Answer:** *(5-7 sentences)*

The most challenging part of this assignment was implementing a clean termination for the `CpuWorker` threads when replacing busy waiting with a counting `Semaphore` in Feature 3. Initially, replacing the polling loop with `availableProcesses.acquire()` successfully reduced `busyWaitPolls` to zero, but the program timed out and triggered the watchdog at the end. This happened because once the final process finished executing, the remaining idle CPU threads stayed blocked inside `acquire()` waiting for permits that would never arrive. Solving this required carefully checking `SharedStats.getCompletedProcessCount() >= SharedStats.totalProcesses` right after a process finished and calling `release(SharedStats.totalCPUs)` to wake every sleeping CPU. Additionally, placing a second completion check immediately after `acquire()` ensured that awakened CPUs exited the loop cleanly instead of polling an empty queue.

## Question 3: How did you overcome the challenges you faced?

**Your Answer:** *(5-7 sentences)*

To overcome these challenges, I followed an incremental approach by implementing and testing one feature at a time rather than changing everything at once. First, I read `SchedulerSimulationSync.java` from top to bottom and traced where `RaceWindow.pause()` was placed inside `SharedStats` and `ReadyQueue` to identify every critical section. Whenever a run behaved unexpectedly—such as the threads hanging on the semaphore—I traced the exact number of `release()` and `acquire()` calls across `main`, `ReadyQueue.add()`, and `CpuWorker.run()`. Running the simulation five consecutive times after each feature helped me verify that my fixes worked deterministically rather than by luck. Finally, keeping separate commits for each step made it easy to isolate bugs and confirm that each synchronization mechanism solved its specific problem.

## Question 4: Where can synchronization concepts be applied in real-world applications?

**Your Answer:** *(5-7 sentences)*

Synchronization concepts like mutex locks and semaphores are essential in almost every multi-user real-world software system. For example, in an online banking application, two simultaneous transfers from the same account form a read-modify-write critical section on the account balance that must be protected by a mutex lock to prevent lost updates. Similarly, airline or concert ticket booking platforms use locks to ensure that two customers cannot reserve the exact same last seat at the same time. Counting semaphores are widely used in database connection pools and web servers to limit how many worker threads can access a fixed number of database connections simultaneously, blocking excess requests instead of busy waiting. Even background print spoolers and operating system task schedulers rely on the exact producer-consumer queue synchronization built in this assignment.

### Optional: What would you like to learn more about?

I would like to learn more about lock-free data structures and Java's `java.util.concurrent` atomic classes (such as `AtomicInteger` and `ConcurrentLinkedQueue`) and how they compare in performance to `ReentrantLock`.

### Optional: How confident do you feel about synchronization concepts now?

Intermediate to Confident. I now have a solid understanding of identifying critical sections, applying `ReentrantLock` with `try/finally`, and coordinating threads with semaphores, though I want more practice debugging complex multi-lock deadlock scenarios.

### Optional: Feedback on the assignment

The built-in `RaceWindow.pause()` and `VERIFICATION` summary table were very helpful because they made concurrency bugs reproducible and immediately showed whether each fix worked.

---

# Part C: Technical Answers (0.5 mark)

## Question 1: Race Condition in Your Own Output

**Your Answer:** *(3-5 sentences)*

In the original starter run with my student ID (`444051957`), multiple shared counters suffered from lost updates because `RaceWindow.pause()` forced a context switch between reading and writing the variables. Specifically, `Context switches`, `Completed processes`, and `Total service time` all showed `✘ MISMATCH` because observed values were lower than expected, and `Busy-waiting polls` was far above zero. On a real machine without `RaceWindow`, the exact same race condition still happens whenever the OS hardware timer preempts a thread during the nanosecond window between reading a variable from memory into a register and writing the incremented result back, making it rare and very hard to reproduce during testing.

Verification block of the **original starter**:

# Part C: Technical Answers (0.5 mark)

> 🛑 **STOP:** You cannot answer these questions without understanding the code. Re-read `SchedulerSimulationSync.java` and **run it** first. Your answers must reference **your own code and your own output** (your student ID makes your output and your expected values unique).
>
> ⚠️ **WARNING:** Each answer must be **3 to 5 sentences**, with specific examples from your code or output. Use correct terms: race condition, critical section, mutual exclusion, mutex lock, semaphore, busy waiting, deadlock, producer, consumer.
>
> 💡 **TIP:** Keep the output of the **original starter** and the output of your **final version** in text files or screenshots, so you can copy real snippets for Question 1.

## Question 1: Race Condition in Your Own Output

**Question**: Run the **original starter** (before any fix) and paste the **verification block** of that run. Which value was wrong (expected vs observed)? Explain **step by step**, with two named threads/CPUs, how **one lost update** happens on one of the shared variables (read, `RaceWindow.pause()`, write). Why can the same bug happen on a real machine even without `RaceWindow`, and why is it hard to detect?

> ⚠️ **WARNING:** The snippet must come from **your own run** (with your student ID), not from a classmate or from this README.
>
> 💡 **TIP:** Use a small timeline: *CPU-1 reads `contextSwitchCount` = 12 → CPU-2 reads 12 → CPU-1 writes 13 → CPU-2 writes 13 → one increment is lost.* If your starter run crashed before printing numbers, run it several times (or paste the exception and the watchdog message and explain it).

**Your Answer:** *(3-5 sentences)*

[Write your answer here.]

Verification block of the **original starter**:
```
[Paste the verification block (or the exception/watchdog message) of the starter here]
```

Verification block of **my final version**:
```
[Paste the verification block of your final version here (all lines ✔)]
```

**Explanation of the timeline:**
[Explain the lost update step by step.]

## Question 2: Critical Sections and Lock Granularity

**Question**: List the **critical sections** you protected (variables and methods) and the lock(s) you used. **Lock granularity:** did you use **one lock** for the three statistics or **one lock per variable**? Why, and what is the trade-off? Why is the **ready queue** protected by a **different** lock than the statistics? Explain how your solution provides **mutual exclusion**, and discuss **progress** and **bounded waiting** (a default `ReentrantLock` is not fair: what does that imply?).

> 💡 **TIP:** The three counters are independent: does updating `contextSwitchCount` need to block an update of `totalServiceTime`? Also think about what could go wrong (deadlock, or long waiting) if the queue lock and the statistics lock were the **same** lock and a thread held it while doing something slow.

**Your Answer:** *(3-5 sentences)*

[Write your answer here.]

| Critical section (variable / method) | Lock used | Why it needs protection |
|---|---|---|
| [e.g., `ReadyQueue.poll()`] | [lock name] | [reason] |
| [...] | [...] | [...] |

## Question 3: Busy Waiting vs Semaphore

**Question**: Describe the **busy waiting** of the starter and its cost (give the `Busy-waiting polls` number from your **starter** run). What does the **value of your semaphore** represent? What is its **initial value** and why? What is its value right after the `numProcesses` initial `add()` calls? Why does the last CPU call `release(totalCPUs)` at the end, and what would happen if it did not?

> 💡 **TIP:** Think about what a CPU does when the queue is empty in the starter, and what a CPU does in your final version (is it running, ready or blocked?). Also check what happens to a CPU blocked in `acquire()` when no process will ever be added again.

**Your Answer:** *(3-5 sentences)*

[Write your answer here.]

## Question 4: Classical Problems and Deadlock

**Question**: The CPUs and the ready queue look like a classical synchronization problem of Chapter 5. **Name it**, and say who plays the **producer** and the **consumer** roles (careful: here the CPUs also re-enqueue processes). If the ready queue were **bounded** (capacity `K`), name the **three semaphores** you would need and their **initial values**. Describe a **deadlock scenario** that appears if a thread acquired the **mutex before** waiting on the semaphore (or if two locks were acquired in different orders), and say **which of the four necessary conditions** you would break to prevent it.

> 💡 **TIP:** Recall the bounded-buffer solution of the slides (`empty`, `full`, `mutex`) and the order of `wait()` calls in the producer and the consumer. For the deadlock, think about a producer that holds the mutex while waiting for a free slot that only a consumer (who needs the mutex) can create.

**Your Answer:** *(3-5 sentences)*

**Classical problem and roles**:
[Name the problem; who is the producer, who is the consumer?]

**Semaphores for a bounded queue (name and initial value)**:
[Name the three semaphores and their initial values.]

**Deadlock scenario and prevention**:
[Describe the scenario and the necessary condition you would break.]

## Summary

**Key concepts I understood through these questions:**
1.
2.
3.

**Concepts I need to study more:**
1.
2.

---

# ✅ Final Checklist (complete before submitting)

> ⚠️ **WARNING:** Go through every line. Blackboard does not accept submissions after the deadline, which is **November 14, 2026**.

**Repository**
- [ ] Repository is **PUBLIC** (Settings → Danger Zone → Visibility)
- [ ] Repository is renamed to `OS-Assignment3-YourFirstName-YourLastName`
- [ ] GitHub account uses the university email (`@std.psau.edu.sa`)

**Code**
- [ ] Student ID is set in `SchedulerSimulationSync.java` (line 304)
- [ ] My code is based **only** on the starter of this repository (nothing copied from previous assignments)
- [ ] Code compiles and runs with no errors, and terminates by itself (no `⛔ WATCHDOG`)
- [ ] Feature 1 (ready queue lock), Feature 2 (statistics locks) and Feature 3 (semaphore, no busy waiting) all work
- [ ] **The four verification lines are ✔ in 5 consecutive runs**
- [ ] Every lock is released in a `finally` block
- [ ] `RaceWindow`, `Config`, the verification block and the watchdog are **unchanged**
- [ ] Each feature has clear comments

**Commits**
- [ ] **At least 4 meaningful commits, ideally 7 or more**
- [ ] **One commit per feature**
- [ ] Commits are spread over **different dates** (not all in the last hour)
- [ ] Everything is **pushed** to GitHub

**This file (`MY_WORK.md`)**
- [ ] Full name and student ID filled in at the top
- [ ] Development log has **5+ entries** on different dates
- [ ] Reflection: 4 questions, 5-7 sentences each
- [ ] Technical answers: 4 questions, 3-5 sentences each, with examples from **your** output (starter output **and** final output pasted in Question 1)
- [ ] No `[...]` placeholders left
- [ ] No section headers deleted

**Video**
- [ ] 2-3 minutes long, named `StudentID_Assignment3_Demo.mp4`
- [ ] Shows your name, ID, repository, 3 features (and your lock granularity choice), IDE execution with the verification block, one synchronization concept, and commit history
- [ ] Link is **public** (tested in an incognito window) and pasted in the **Video Link** section above

**Blackboard**
- [ ] Submit **only** the link to your public GitHub repository

> 🎯 **Good luck!** Start early, commit regularly, and make sure you can explain every line you submit.
