---
layout: page
permalink: /research/
title: Research
nav: true
nav_order: 1
---

<div class="research-page">

  <section class="research-hero" aria-labelledby="research-thesis">
    <div class="research-hero-copy">
      <p class="research-eyebrow">Probabilistic modeling and optimization</p>
      <h2 id="research-thesis" class="research-thesis">Scalable machine learning with gradients and curvature</h2>
      <p class="research-lead">
        Gradients and curvature information characterize how functions and loss landscapes change
        locally. Gradient observations can sharpen probabilistic predictions and
        uncertainty estimates and guide sequential decisions in Bayesian optimization,
        while curvature can correct for anisotropy and improve conditioning in
        neural network training. The main obstacle is computational. In standard dense formulations, covariance and curvature matrices require
        quadratic storage and cubic-time factorization or inversion.
      </p>

      <p class="research-lead">
        My research develops scalable representations that preserve the benefits of gradients and
        curvature on a prediction or update while avoiding this dense linear algebra.
      </p>
    </div>

    <div class="research-overview" aria-label="Research program overview">
      <div class="research-overview-step">
        <span class="research-overview-label">Derivative Gaussian Processes and Bayesian Optimization</span>
        <span>Gradient-informed probabilistic learning for scalable inference and
        high-dimensional decision making</span>
      </div>    
      <div class="research-overview-arrow" aria-hidden="true">↑</div>
      <div class="research-overview-step">
        <span class="research-overview-label">Zeroth-order LLM Fine-Tuning</span>
        <span>Memory-efficient, curvature-aware optimization without backpropagation</span>
      </div>  
      <div class="research-overview-arrow" aria-hidden="true">↑</div>
      <div class="research-overview-step">
        <span class="research-overview-label">Second-order optimization</span>
        <span>Low-rank curvature approximations for scalable gradient preconditioning</span>
      </div>
    </div>
  </section>

<section
  class="research-feature research-feature--wide research-feature--derivatives"
  aria-labelledby="derivative-learning"
>
  <header class="research-feature-header">
    <p class="research-section-kicker">Independent research program</p>

    <h2 id="derivative-learning">
      Derivative-informed probabilistic modeling
    </h2>

    <p class="research-key-idea">
      <strong>Key idea.</strong>
      Predict the scalar response without carrying the entire gradient state.
    </p>
  </header>

  <figure
    class="research-visual research-visual--tera"
    role="img"
    aria-label="TERA target-specific gradient reduction"
  >
    <img
      src="{{ '/assets/img/research/tera-method-panel.png' | relative_url }}"
      alt="TERA target-specific gradient reduction for derivative Gaussian processes."
      loading="lazy"
      decoding="async"
    >

    <figcaption>
      Each conditioning gradient affects the target conditional only through its
      projection onto the span of target-centered input differences.
    </figcaption>
  </figure>

  <div class="research-feature-body">
    <div class="research-feature-narrative">
      <p>
        Gradient observations can substantially improve Gaussian process (GP)
        surrogates, but standard derivative GPs treat all gradient
        coordinates at each location as separate responses. Their covariance
        blocks therefore scale with both sample size and input dimension.
      </p>

      <p>
        For stationary kernels, the gradient components relevant to a target function
        value lie in the span of target-centered input differences. Within each Vecchia
        conditional, the full conditioning gradients can therefore be replaced by
        reduced directional derivatives without changing the corresponding
        full-gradient conditional density.
      </p>

      <p>
          Because the reduction is exact within each Vecchia conditional, the Vecchia
          approximation is the only source of discrepancy from the full derivative GP.
          Direct construction of the reduced conditional factors avoids forming or
          factorizing full derivative covariance blocks. This makes derivative GP
          inference practical for large datasets and high-dimensional problems and
          enables its use in Bayesian
          optimization.
      </p>
    </div>

    <div class="representative-work">
      <span class="representative-label">Representative work</span>

      <strong>
        Scalable Derivative Gaussian Processes via Exact Gradient Reduction
      </strong>

      <span class="representative-links">
        <a href="https://doi.org/10.48550/arXiv.2606.02909">Paper</a>
        <span aria-hidden="true">·</span>
        <a href="https://github.com/hseung88/tera">Code</a>
      </span>
    </div>
  </div>
</section>

  <section
    class="research-feature research-feature--wide research-feature--curvature"
    aria-labelledby="structured-curvature"
  >
    <header class="research-feature-header">
      <p class="research-section-kicker">Foundational research program</p>

      <h2 id="structured-curvature">
        Curvature-aware deep learning optimization
      </h2>

      <p class="research-key-idea">
        <strong>Key idea.</strong>
        Exploiting low-rank structure enables efficient approximations of dominant
        curvature geometry.
      </p>
    </header>

    <figure
      class="research-visual research-visual--curvature research-visual--loren"
      role="img"
      aria-label="LOREN optimization trajectories on the monkey-saddle objective"
    >
      <img
        src="{{ '/assets/img/research/loren-monkey-saddle.png' | relative_url }}"
        alt="Optimization trajectories of first- and zeroth-order methods on a monkey-saddle objective, with LOREN shown in blue."
        width="574"
        height="424"
        loading="lazy"
        decoding="async"
      >

      <figcaption>
        On the monkey saddle, LOREN follows a more direct escape path than the
        zeroth-order (ZO) baselines by combining low-rank curvature with variance-reduced
        ZO gradient estimates.
      </figcaption>
    </figure>

    <div class="research-feature-body">
      <div class="research-feature-narrative">
        <p>
          The dominant geometry of the layer-wise Fisher information in neural networks is well
          approximated by a rank-one structure defined by the mean activation. This
          yields a closed-form preconditioner that captures useful curvature
          without storing dense covariance matrices or performing costly matrix
          inversions.
        </p>

        <p>
          The same structural principle shifts from preconditioning observed gradients
          to designing perturbation queries when gradients are unavailable. Each pair of
          function evaluations measures loss variation along a sampled direction,
          providing a finite-difference approximation to a directional derivative. A
          block-diagonal rank-one approximation to inverse curvature parameterizes an
          anisotropic Gaussian distribution over these directions, so that queries follow
          learned local geometry rather than isotropic perturbations. This yields
          curvature-aware zeroth-order optimization with only vector-sized auxiliary
          state and without explicit Hessian estimation.
        </p>
      </div>

      <div class="representative-work representative-work--stacked">
        <span class="representative-label">Representative work</span>

        <div>
          <strong>
            Low-Rank Curvature for Zeroth-Order Optimization in LLM
            Fine-Tuning
          </strong>
          <span class="representative-links">
            <a href="https://doi.org/10.1609/aaai.v40i30.39715">Paper</a>
            <span aria-hidden="true">·</span>
            <a href="https://github.com/hseung88/loren">Code</a>
          </span>
        </div>

        <div>
          <strong>
            MAC: An Efficient Gradient Preconditioning using Mean Activation
            Approximated Curvature
          </strong>
          <span class="representative-links">
            <a href="https://doi.org/10.1109/ICDM65498.2025.00077">Paper</a>
            <span aria-hidden="true">·</span>
            <a href="https://github.com/hseung88/mac">Code</a>
          </span>
        </div>
      </div>
    </div>
  </section>

  <p class="research-closing">
    My broader goal is to enable the practical use of gradients and curvature at
    modern scale by reducing computational cost while improving sample and
    optimization efficiency.
  </p>

</div>
