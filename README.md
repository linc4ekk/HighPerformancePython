# HighPerformancePython
Solutions of tasks in High Performance Python Lab course at Skoltech

**Task 1**: Bifurcation map

Plot classical bifurcation map. $x_{n+1} = r * x_n * (1 - x_n)$ where $x_0 = rand(0, 1)$, $r$ - const.

| | Criteria name  | Max score |
| -- | ------------- | ------------- |
|T1.1| Implement the map, plot the evolution of x | 1 |
|T1.2| Create a linspace of r’s, for every r save the last “m” values of x after the first “n” values, play around with values | 1 |
|T1.3| Get the bifurcation map | 1 |
|T1.4| Parallel computations | 2 |
|    | Plot speedup versus number of processors graph | 2 |


**Task 2**: Julia set


| | Criteria name  | Max score |
| -- | ------------- | ------------- |
|T2.1| Generate black and white image  | 1 |
|T2.2| Use different color for bifurcation points | 1 |
|T2.3| Mandelbrot set  | 2 |
|T2.4| Plot some figures for c = exp(i * alpha), alpha in range(0, 2pi) | 2 |
|T2.5| Plot gif of figures for c = exp(i * alpha), alpha = range(0, 2pi) | 2 |


**Task 3** Schelling model


Ganeral: figsize = (14, 11), fontsize = 20.
| | Criteria name  | Max score |
| -- | ------------- | ------------- |
|T3.1| 9 gifs for 9 values of R  | 1 |
|T3.2| Plot # of moving cells vs times for 9 values of R | 1 |

**Task 4**:  Spectrogram

**Task 5**: Matmul

Measure time of different matrix multiplication functions

**Task 6**: Advanced Spectrogram

Use Jupyter notebook templates to make something mre interesting

| | Criteria name  | Max score |
| -- | ------------- | ------------- |
|T6.1| Add fourth wave packets of harmonic signal (frequency=4 and time_shift=7 cycles). See how to adjust frequency and time shift of signal by using, e.g., figures about AFP and STFT. These figures give you information about the amplitudes, frequencies, signal longitudes and signal time. You may see it like "cause & effect", where "cause" is to change some parameters of forming signal and "effect" are consequent changes in figures | 1 |
|T6.2| Explain, why the "hats" of signal and AFP may be sharp | 1 |
|T6.3| Vary kappa on [0.001, 10], kappa=exp(theta), theta=linspace(ln(0.001), ln(10), 100 steps), create GIFs| 1 |
|T6.3| Explain, why specgram is different| 1 |
|T6.4| PVary n_timestamps_given=4090, 4091, ...,5000 and plot results of computational time on the graph. | 2 |
| | Explain why cProfiler gives different results. What is the bottleneck in this program? How can you improve the program? | 2 |
|T6.5| Parallel STFT | 2 |	
| | Plot speedup versus number of processors graph |	2 |

**Task 7**: Study an integral

- Compute an integral using the trapezoid rule
- Split the job between processes and use Reduce collective communication
- Check the accuracy when taking more nodes (i.e. smaller step)
- Check the speedup when taking more processes
![integral](https://github.com/zakajd/HighPerformancePython/blob/master/imgs/integral.png)
