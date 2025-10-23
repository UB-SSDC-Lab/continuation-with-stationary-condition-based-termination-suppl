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

Results are showcased for two of the three examples from the paper. First, a minimum-fuel transfer between L2 and L1 halo orbits, where the videos step through freeing the terminal-halo parameter $(s_1)_f$, the initial-halo parameter $(s_1)_0$, and finally the final time $t_f$; the resulting solution reorganizes thrust/coast structure and exploits the unstable invariant manifolds of the initial L2 halo orbit. Second, a minimum-time transfer from GTO to the L1 halo manifold, where successive stages free $s_1$, $s_2$, the initial true-longitude parameter $s_\omega$ ($\omega_{0,\text{true}}=2\pi s_\omega$), and the initial true anomaly parameter $s_\theta$ ($\theta_0=2\pi s_\theta$). These animations highlight how PALC navigates folds and sensitivity in many-revolution spirals while the termination criterion ensures each stage can progress until reaching the desired optimum. 

Collectively, the clips make visible how the trajectories and optimal control cost functions change while each parameter is freed from initial “fixed-parameter” solutions to the final desired ones.  

## Transfer Between Halo Orbits with Minimum-Fuel

### Continuation of $(s_1)_f$ parameter

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="800" controls>
        <source src="/assets/L2_halo_to_L1_halo_sf_continuation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the s<sub>f</sub> parameter for transfer between L2 and L1 halo orbits</em></p>
</div>
~~~

### Continuation of $s_0$ parameter

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="800" controls>
        <source src="/assets/L2_halo_to_L1_halo_s0_continuation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the s<sub>0</sub> parameter for transfer between L2 and L1 halo orbits</em></p>
</div>
~~~

### Continuation of $t_f$ parameter

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="800" controls>
        <source src="/assets/L2_halo_to_L1_halo_tf_continuation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the t<sub>f</sub> parameter for transfer between L2 and L1 halo orbits</em></p>
</div>
~~~

## Transfer from GTO to an L1 Halo Orbit in Minimum-Time

### Continuation of $s_1$ parameter

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

~~~
<div style="text-align: center; margin: 2em 0;">
    <video width="1000" controls>
        <source src="/assets/step4_animation.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    <p><em>Animation showing the continuation of the s<sub>&#952;</sub> parameter for transfer from GTO to an L1 halo orbit</em></p>
</div>
~~~
