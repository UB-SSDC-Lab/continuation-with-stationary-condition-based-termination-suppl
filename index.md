+++
title = "Continuation with Stationary Condition-Based Termination Supplementary Animations"
hasmath = true
hascode = false
+++

~~~
<!-- Main "about me" section -->
<br>
<!-- Centered title and authors -->
<div style="text-align: center; max-width: 800px; margin: 0 auto;">
    <h1 class="title" style="text-align: center;">Continuation with Stationary Condition-Based Termination Supplementary Animations</h1>
    <l>Grant R. Hecht, Dylan M. LaSalle, and Eleonora M. Botta</l>
</div>

<!-- Left-justified content -->
<div style="text-align: left; max-width: 800px; margin: 1.5em auto 0 auto;">
    <p>
    This website contains supplementary animations and discussion for the publication:
    </p>
    <p style="font-style: italic; margin-bottom: 1.5em;">
    G. R. Hecht, D. M. LaSalle, and E. M. Botta, "Continuation with Stationary Condition-Based Termination for Optimal Orbit Transfer Problems," <em>IEEE Transactions on Aerospace and Electronic Systems</em> (ADD PUBLICATION INFO).
    </p>

    <div style="text-align: center;"><a href="mailto:ebotta@buffalo.edu.edu">email</a>&ensp;//&ensp;<a href="https://ubssdclab.wixsite.com/ssdclabmobile">website</a>&ensp;//&ensp;<a href='https://github.com/UB-SSDC-Lab'>github</a></div>
</div>
<br>
~~~

## Overview
The animations on this page illustrate our continuation framework for optimal low-thrust trajectory design, which couples pseudo-arclength continuation (PALC) with a stationary-condition–based termination rule. In each stage, we track a zero-curve of a parameterized shooting function and halt exactly when the transversality (stationary) condition for the active continuation parameter is satisfied—yielding an optimal solution to the final desired problem.  

Results are showcased for two of the three examples from the paper. First, a minimum-fuel transfer between $\text{L}_2$ and $\text{L}_1$ halo orbits, where the videos step through freeing the terminal-halo parameter $(s_1)_f$, the initial-halo parameter $(s_1)_0$, and finally the final time $t_f$; the resulting solution reorganizes thrust/coast structure and exploits the unstable invariant manifolds of the initial L2 halo orbit. Second, a minimum-time transfer from GTO to the $\text{L}_1$ halo manifold, where successive stages free $s_1$, $s_2$, the initial true-longitude parameter $s_\omega$ ($\omega_{0,\text{true}}=2\pi s_\omega$), and the initial true anomaly parameter $s_\theta$ ($\theta_0=2\pi s_\theta$). These animations highlight how PALC navigates folds and sensitivity in many-revolution spirals while the termination criterion ensures each stage can progress until reaching the desired optimum. 

Collectively, the clips make visible how the trajectories and optimal control cost functions change while each parameter is freed from initial “fixed-parameter” solutions to the final desired ones. In each animation, the panels showing the stationary-condition function  (i.e., $c_i$ $i\in\{0,1,2,3\}$) and the corresponding optimal-control cost (i.e., $\Delta m$ or $\Delta t$) include a moving marker that traces the current solution point along the zero curve, synchronized with all other panels.

## Transfer Between Halo Orbits with Minimum-Fuel

This example corresponds to the minimum-fuel $\text{L}_2$ to $\text{L}_1$ halo orbit transfer discussed in Section IV-B of the paper. The sequence of animations illustrates how the stationary-condition–based continuation method transitions the initial fixed-parameter problem to the fully free final-time formulation. Each stage frees one parameter of the boundary-value problem while pseudo-arclength continuation tracks the corresponding zero-curve and terminates automatically at the transversality point.

### Continuation of $(s_1)_f$ parameter

This first stage frees the terminal-halo parameter $(s_1)_f$, allowing the trajectory to converge toward the optimal arrival location on the $\text{L}_1$ halo. As shown in the animation, the insertion point on the target halo orbit gradually shifts as the continuation parameter is varied, leading to noticeable changes in the overall trajectory. The placement and timing of the thrust arcs also evolve throughout the process, as evident in the top-center panel.

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="1000" controls>
        <source src="/assets/L2_halo_to_L1_halo_sf_continuation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the s<sub>f</sub> parameter for transfer between L2 and L1 halo orbits</em></p>
</div>
~~~

### Continuation of $s_0$ parameter

The second stage frees the initial-halo parameter $(s_1)_0$, enabling optimization of both the departure from the $\text{L}_2$ orbit and the arrival at the $\text{L}_1$ orbit. As the continuation parameter $(s_1)_0$ is varied, the exit point from the initial halo orbit moves steadily, producing corresponding adjustments in the overall trajectory. Interestingly, the final insertion point on the target halo also shifts to remain optimal—ultimately returning toward the initially prescribed location.

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="1000" controls>
        <source src="/assets/L2_halo_to_L1_halo_s0_continuation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the s<sub>0</sub> parameter for transfer between L2 and L1 halo orbits</em></p>
</div>
~~~

### Continuation of $t_f$ parameter

In the final stage, the continuation frees the final-time parameter $t_f$, completing the transition to the fully optimal transfer solution. As $t_f$ increases along the zero curve, the departure point from the $\text{L}_2$ halo orbit changes significantly, and the structure of the thrust arcs adapt accordingly. One thrust arc disappears entirely at the point where the slope of the $c_2$ is discontinuous, while the initial thrust arc diminishes until it closely resembles an impulsive maneuver.

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="1000" controls>
        <source src="/assets/L2_halo_to_L1_halo_tf_continuation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the t<sub>f</sub> parameter for transfer between L2 and L1 halo orbits</em></p>
</div>
~~~

## Transfer from GTO to an L1 Halo Orbit in Minimum-Time

This example corresponds directly to the minimum-time GTO→L₁ manifold transfer presented in Section IV-C of the paper. The animations display the evolution of the trajectory throughout the continuation process in which the parameters $s_1$, $s_2$, $s_\omega$ ($\omega_{0,\text{true}}=2\pi s_\omega$), and $s_\theta$ ($\theta_0=2\pi s_\theta$) are successively freed. Each stage traces the corresponding zero-curve using pseudo-arclength continuation and terminates automatically when the transversality condition is satisfied. The progression clearly shows how the spiral geometry evolves and the transfer time decreases as the continuation advances toward the optimal minimum-time solution of the desired problem.

### Continuation of $s_1$ parameter

The first stage frees $s_1$, transitioning the trajectory to the optimal insertion into the prescribed cross-section of the $\text{L}_1$ halo’s stable manifold. As noted in the paper, this stage moves from a local maximum of the initial problem to a nearby local minimum. In the animation, the Earth-centered spirals visibly rotate as the final insertion point moves along the cross-section, and the terminal coast on the stable manifold adjusts accordingly.

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="1000" controls>
        <source src="/assets/step1_animation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the s<sub>1</sub> parameter for transfer from GTO to an L1 halo orbit</em></p>
</div>
~~~

### Continuation of $s_2$ parameter

Freeing $s_2$ then refines the insertion onto the stable manifold. Only modest geometric changes are observed, but the Earth-centered revolutions show slight rotation, and the insertion point shifts closer to Earth, consistent with the incremental improvement reported in the paper and shown in the right panel.

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="1000" controls>
        <source src="/assets/step2_animation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the s<sub>2</sub> parameter for transfer from GTO to an L1 halo orbit</em></p>
</div>
~~~

### Continuation of $s_\omega$ ($\omega_{0,\text{true}}=2\pi s_\omega$) parameter

This stage frees the initial true-longitude of perigee parameter $s_\omega$, allowing the GTO’s orientation to vary. As $s_\omega$ changes, the Earth-centered spirals rotate markedly—briefly reversing direction as PALC traverses folds on the zero-curve—and the final coast along the stable manifold decreases appreciably.

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="1000" controls>
        <source src="/assets/step3_animation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the s<sub>&#969;</sub> parameter for transfer from GTO to an L1 halo orbit</em></p>
</div>
~~~

### Continuation of $s_\theta$ ($\theta_0 = 2\pi s_\theta$) parameter

The final stage frees the true-anomaly parameter $s_\theta$, completing the continuation to the desired minimum-time solution. Only minor rotation in the spirals are visible, consistent with the small additional reduction in time of flight achieved in this step.

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="1000" controls>
        <source src="/assets/step4_animation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the s<sub>&#952;</sub> parameter for transfer from GTO to an L1 halo orbit</em></p>
</div>
~~~
