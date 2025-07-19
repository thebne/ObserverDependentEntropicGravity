# Entropy-Observer Duality: An Interactive Research Sketch on Galaxy Rotation Curves

This repository contains a Jupyter notebook (`entropy_observer_duality_sketch.ipynb`) exploring an intuitive theory of entropy-observer duality applied to galaxy rotation curves. It's a personal, enthusiast-level experiment to test if a relational view of time and gravity—framed through information trades—can refine existing models like Verlinde's entropic gravity.

## Premise
The core idea is a duality where time emerges from "holding distinctions" (maintaining asymmetries against chaos through sequential resolutions, like noticing environmental disorder), and gravity from "distinctions you can observe but haven't yet" (potential to average external asymmetries, pulling toward merging). This is recursive: Horizons hide nested micro-evolutions with "slower" internal time for efficient rearrangement, driving a "survival of the fittest" for observers that persist by evolving local symmetries.

Inspired by entropic gravity and holography, but kept abstract—it's not claiming novelty, just framing to make sense of why time and gravity feel info-linked.

## What We're Trying to Do
We use the SPARC dataset (high-quality rotation curves for 175 galaxies) to fit three models:
- **Newtonian**: Baseline gravity from baryonic mass (predicts declining curves, but data is flat).
- **Verlinde Approximation**: Entropic modification for emergent "dark" effects (sqrt(g_bar * a0) term).
- **Feedback (Recursive)**: Our addition—a scale-dependent term g_fb = beta * exp(-r / r0) capturing the duality's resync loop (desync exposure invites pulls, damped recursively across nested horizons).

The notebook processes all galaxies, computes fit quality (reduced chi^2), breakdowns by category (e.g., low-surface-brightness dwarfs), and correlations (beta/r0 vs. mass/density). Interactive plots let you visualize individual fits.

## Why?
To empirically probe the duality: If feedback systematically lowers chi^2 (better matches flat curves without dark matter), it hints the relational loop adds value—e.g., variable resyncs for non-orderly galaxies (sparse desyncs need damping for persistence). It's a sketch to "grok" unification: Time as desync flow, gravity as resync metric, with recursion explaining dilation/redshifts. Results show ~73% chi^2 drop vs. previous forms, stronger in disordered dwarfs—encouraging for the "fittest observers" intuition.

This is exploratory, not rigorous—flaws like high residual chi^2 suggest missing baryonics, but it's a fun way to test ideas.

## Setup
1. Download SPARC data: Rotation curves (*.rotmod.dat) and master table (SPARC_Lelli2016c.mrt) from [astroweb.case.edu/SPARC](http://astroweb.case.edu/SPARC/).
2. Place in `data/sparc/` folder.
3. Install dependencies: `pip install numpy scipy matplotlib pandas ipywidgets`.
4. Run the notebook in Jupyter.

## Usage
- Open `entropy_observer_duality_sketch.ipynb`.
- Run cells top-to-bottom.
- Use interactive dropdown to plot specific galaxies.
- Extend: Tweak feedback_form ('exp' or '1/r') or add gas fraction correlations.

## Results Summary
From full run (July 19, 2025):
- Avg chi^2: Newton 261.66, Verlinde 115.97, Feedback 11.85.
- Feedback better: 93.1% vs Verlinde, 94.3% vs Newton.
- Categories: Strongest gains in LSB dwarfs (70.2% improvement, low chi^2 ~7.22).
- Correlations: Beta anticorrelated with density (r=-0.677 Sigma_e), r0 positive with mass (r=0.252 log(Mbar))—aligning with symmetry evolution.

## Limitations
- Simplified models; real fits need 3D baryonics/outflows.
- Assumes SPARC accuracy; errors in mass/surface brightness affect categories.
- Not peer-reviewed—enthusiast sketch for intuition, not publication.

## References
- SPARC Dataset: Lelli et al. (2016), ApJL 827, L19.  (galactic-spin-W1 repository)
- Entropic Gravity: Verlinde (2011), JHEP 04, 029.
- Inspired by: Jacobson thermodynamics, holographic duality.

Feedback welcome, feel free to fork/contribute!