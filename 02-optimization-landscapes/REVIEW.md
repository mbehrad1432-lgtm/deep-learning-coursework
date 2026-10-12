# Static review

- optimize_loss receives params but evaluates loss_func(x,y) using globals.
- start_x/start_y and epochs are also notebook globals.
- Plots call detach().numpy() directly, assuming CPU tensors.
- Newton solves the raw Hessian; singular or indefinite curvature can fail or lead away from a minimum.
- Trajectory comparisons use illustrative initial points/settings and do not establish a universal optimizer ranking.

## Supplied revisions

- Computed objective from supplied parameters rather than global x/y.
- Plot starting point, epochs and CPU assumptions still come from notebook globals.

Only structural schema/syntax checks were performed. No fresh model scores, gradient-test outcomes, runtime benchmarks or successful Run-All claim is made.
