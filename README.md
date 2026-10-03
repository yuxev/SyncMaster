<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/banner-dark.svg" />
  <img src="docs/banner-light.svg" width="100%" alt="SyncMaster: The dining philosophers with pthreads and mutexes, plus a bonus built on processes and semaphores." />
</picture>

SyncMaster or Table of Threads in this projects i developed a simulation inspired by the "Dining Philosophers" problem to explore concurrency, race conditions, and resource management in multithreaded environments. The project required managing shared resources among multiple "philosophers" (threads) who alternated between thinking and eating. The focus was on preventing race conditions, avoiding deadlocks, and ensuring no starvation of threads. By utilizing mutexes and semaphores, I implemented efficient synchronization mechanisms to guarantee thread safety and proper resource allocation. This project significantly enhanced my skills in concurrent programming, thread synchronization, and the prevention of common pitfalls like race conditions and deadlocks.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/table-dark.svg" />
  <img src="docs/table-light.svg" width="100%" alt="Five philosophers around a table; each fork is a mutex; P1 locks fork 1 then fork 2" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/timeline-dark.svg" />
  <img src="docs/timeline-light.svg" width="100%" alt="Gantt chart of ./philo 5 800 200 200 showing eating, sleeping and thinking" />
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/bonus-dark.svg" />
  <img src="docs/bonus-light.svg" width="100%" alt="Bonus version: parent process forks one child per philosopher; forks are a named semaphore" />
</picture>

## Run it

```bash
cd philo && make
./philo 5 800 200 200        # philosophers, time_to_die, time_to_eat, time_to_sleep (ms)
./philo 5 800 200 200 7      # optional: stop once everyone has eaten 7 times
cd ../philo_bonus && make && ./philo_bonus 5 800 200 200
```

<sub>Diagrams in <code>docs/</code> are generated SVGs, drawn to match the code in this repo.</sub>
