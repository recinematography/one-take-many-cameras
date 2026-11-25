# One Take, Many Cameras: Audio-Grounded Shot Synthesis for Dialogue Re-Cinematography

[Anthony Chen](https://atchen.com)<sup>1,2*</sup>, [Naomi Ken Korem](https://github.com/Naomi-Ken-Korem)<sup>2</sup>, [Matan Ben-Yosef](https://github.com/matanby)<sup>2</sup>, [Tavi Halperin](https://tavihalperin.me/)<sup>2</sup>, [Urska Jelercic](http://www-f1.ijs.si/~urska/)<sup>2</sup>, [Ofir Bibi](https://github.com/ofirbb)<sup>2</sup>, [Daniel Cohen-Or](https://danielcohenor.com/)<sup>3</sup>, [Or Patashnik](https://orpatashnik.github.io/)<sup>3</sup>, [Maneesh Agrawala](https://graphics.stanford.edu/~maneesh/)<sup>1</sup>

<sup>1</sup>Stanford University &nbsp; <sup>2</sup>LTX &nbsp; <sup>3</sup>Tel Aviv University

<sup>*</sup>Work done during a visit to Stanford University and an internship at LTX.

[![arXiv](https://img.shields.io/badge/arXiv-2611.33147-b31b1b.svg)](http://arxiv.org/abs/2611.33147)
[![Project page](https://img.shields.io/badge/Project-Page-blue)](https://recinematography.github.io)

## Code

Code coming soon.

## Abstract

Creating a dialogue scene typically requires cutting between multiple views (e.g., close-ups, medium shots, and over-the-shoulder shots) of the actors. Yet capturing such coverage is costly and in many settings unavailable. We study *dialogue re-cinematography*: synthesizing additional shots from a single wide-angle dialogue video. Existing video generators can synthesize new shots, but rely on visual cues alone, so when the source video barely shows the lips, the generated lip motion fails to match the speech. Our key observation is that the speech audio is view-invariant: it constrains lip motion in any target view. Building on this insight, we adapt a pretrained audio-visual diffusion model to generate the new shot from a target frame that specifies the view, a source video that contains the performance, and the speech audio that drives lip motion. In multi-person scenes, however, pretrained audio-visual models drive every visible face with the same speech, causing *speech leakage*, where silent listeners mouth the speaker’s words. We therefore introduce speaker-aware audio gating, a training-free module that lets the audio drive only the faces that speak in the target shot. On a cinematic paired-view benchmark spanning diverse viewpoints and framings, our method lowers perceptual error by 59%, landmark error by 56%, and speech leakage by 97% relative to the strongest baseline, Wan 3.0. Our method also remains robust on in-the-wild scenes, highlighting its potential for film post-production.

## Citation

```bibtex
@article{chen2026onetake,
  title   = {One Take, Many Cameras: Audio-Grounded Shot Synthesis for Dialogue Re-Cinematography},
  author  = {Chen, Anthony and Ken Korem, Naomi and Ben-Yosef, Matan and Halperin, Tavi and Jelercic, Urska and Bibi, Ofir and Cohen-Or, Daniel and Patashnik, Or and Agrawala, Maneesh},
  journal = {arXiv preprint arXiv:2611.33147},
  year    = {2026}
}
```
