# rusty-task

#### A Rust Based Task Scheduler for Out of Core Scientific Computing

Can we create something like Dask but for scientific computing in Rust? Out of core scientific computing is vital for a large variety of numerical computations, and useful for deployment to a diverse set of hardware. As we are developing Rust based linear algebra tools, and derived parallel software, it would be useful to explore whether a Rust based task scheduler would give us access to high-performance out of core computing with our codes.


### Tasks

- [] Create a Rust interface for delayed funcs
- [] Task graph generator
- [] Task graph visualizer
- [] Scheduler
- [] Linear algebra functionality via [blocked algorithms](https://nhigham.com/2021/10/28/what-is-a-blocked-algorithm/)



### Existing software

- [Tokio](https://tokio.rs/) - an async runtime for Rust, not suitable for scientific computing where we're more interested in out-of-core computing for large tasks, rather than a large number of small O(ms) tasks.



### Literature review

- [Dask: Parallel Computation with Blocked algorithms and Task Scheduling, M. Rokhlin, 2015](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.825.5314&rep=rep1&type=pdf)
	- Overview of Dask vs 0.1.0 API and idea.

- [Parallel and Distributed Computing in Python with Dask, Borbeau, McCarty and Pothina, 2020](https://www.youtube.com/watch?v=EybGGLbLipI&ab_channel=Enthought)
	- Dask tutorial for users, documents the API.

### Questions

- What is a good format for on disk data for a MVP? HDF5? Are there alternatives?? (NetCDF?)

