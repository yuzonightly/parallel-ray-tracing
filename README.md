Use PThreads and MPI to parallelize a simple ray tracing algorithm.

## Run

### hybrid_version

```bash
mkdir build && cd build
cmake ..
make
mpirun -np <number of processes> ./ray_tracing_one_week --threads <number of threads> --scene earth earth.ppm
```

### mpi_version

```bash
mkdir build && cd build
cmake ..
make
mpirun -np <number of processes> ./ray_tracing_one_week --scene earth earth.ppm
```

### sequential_version

```bash
mkdir build && cd build
cmake ..
make
./ray_tracing_one_week --scene earth earth.ppm
```

### thread_version

```bash
mkdir build && cd build
cmake ..
make
./ray_tracing_one_week --threads <number of threads> --scene earth earth.ppm
```
