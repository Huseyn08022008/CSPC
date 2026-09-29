# CSPC

## PW1 --- Lab B

### Results

The observed count decreases approximately exponentially with time. The data follows the expected decay trend, although there are small fluctuations around the analytical law, especially at later times when the count becomes small.

The observed data matches the analytical decay law reasonably well, with deviations consistent with statistical fluctuations in the measurements.

### Snakemake pipeline

The Snakemake pipeline takes the observed decay data as input and runs the plotting script to generate the final figure automatically.



# PW2 Lab A

## Part 3 — The Noise Problem

Acceleration is much noisier than position because differentiation amplifies small measurement noise, and acceleration is obtained by differentiating the data twice.

The mean acceleration was approximately -9.81 m/s², while the standard deviation was large, showing that the acceleration values fluctuate significantly because of noise amplification during differentiation.

## Part 4 — Integrating Back

Integration is the reverse of differentiation. We integrated the noisy acceleration to recover velocity, and then integrated velocity to recover position.

Integration partly suppresses random noise because positive and negative fluctuations can cancel out during the summation.

The recovered position was close to the original position, with a difference of about one metre.

## Part 5 — Plot and Report

The final figure contains three panels:

1. Position versus time
2. Velocity versus time
3. Acceleration versus time

The position is smooth, the velocity is slightly noisy, and the acceleration is very noisy because differentiation amplifies measurement noise.

The final figure was saved as `motion.png`.

### Results

- Mean acceleration: -8.58 m/s²
- Standard deviation of acceleration: 28.72 m/s²
- Largest difference in recovered position: 0.785 m

### Noise observation

The acceleration data is noisy because numerical differentiation amplifies
small measurement errors and random noise. This makes the acceleration much
rougher than the original position data.

Integrating the noisy acceleration back to velocity and then position
partly suppresses the noise. The recovered position was close to the
original position, with a largest difference of about 0.785 m.
