# Short Performance Analysis

### Which version was fastest?

The **sequential** version was the fastest. The parallel version was slower due to the overhead of creating processes and gathering up results. The following image is what I have recorded at the result table. (It slightly changes every run though, but same outcome.)

<img width="251" height="128" alt="image" src="https://github.com/user-attachments/assets/384677f9-54c9-4a83-9099-74039f81c579" />

### What was the speedup achieved?

The speedup achieved was: `0.6223320958742791` using the computation of serial_time / parallel_time. 

### Was efficiency high or low? Why?

The efficiency was `0.0837393465586087` which I think is a low number. Most of the CPU runtime was wasted on overhead. It took too much time splitting data, managing processes, and combining results rather than the actual computation.

### What bottleneck did profiling reveal?

From what I previously mentioned, the `compute_sum()` function bottlenecks due to iterating over a whole lot of numbers that squares and sums it.

### How did optimization affect performance?

From my experience, optimizing the manual function did help, not totally, but made it slightly faster and reduced overhead. I could say it did result to a better performance compared to the unoptimized version.
