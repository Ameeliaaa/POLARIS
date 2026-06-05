# POLARIS: A sub-meter RGB--NIR benchmark with dual-stage spectral-prior injection for joint ice--snow--water mapping in inhabited circumpolar regions

Yongqi Sun, Chenguang Dai, Ruihua Lu, Song Ji, Yu Su, Anzhu Yu

_Submitted to ISPRS Journal of Photogrammetry and Remote Sensing_

---

## Abstract

Joint mapping of ice, snow, and liquid water across inhabited circumpolar regions underpins cryospheric science and infrastructure management. Existing public benchmarks lack the spatial resolution and class scheme required for sub-meter analysis. We present POLARIS, to our knowledge the first sub-meter optical and near-infrared benchmark designed for this task. On POLARIS, an empirical spectral-separability analysis identifies snow versus ice as the only cryospheric class pair without a strongly discriminative spectral index. This finding motivates the integration of class-level priors with spatial reasoning. We further propose dual-stage spectral-prior injection (DSPI), the first framework to couple a class-conditional spectral prior into both the training target and the inference decision for this task. Its spectral-prior modules are decoupled from encoder and decoder internals, so they pair with different RGB and NIR segmentation encoders without architecture-specific changes. Experiments across various encoders show that DSPI consistently improves multimodal mIoU over the corresponding baselines. Across encoders, the per-class IoU pattern and the confusion analysis jointly indicate reduced snow versus ice errors after DSPI. POLARIS closes a sub-meter benchmark gap for inhabited circumpolar regions, and DSPI establishes that measured spectral statistics transfer across segmentation backbones to improve mapping accuracy.

---

## POLARIS Dataset and Code

This repository will provide:

- POLARIS: a sub-meter RGB--NIR benchmark for joint ice, snow, and water mapping in inhabited circumpolar regions, including JL-1 optical imagery at 0.5--0.75 m, co-registered NIR bands, and four-class semantic annotations
- Reference implementations of the dual-stage spectral-prior injection (DSPI) framework for RGB--NIR semantic segmentation

**The dataset and code will be released after the paper is accepted.** Please see the code and `docs/` (if provided) for details on data format, training scripts, and evaluation protocols.

---

## Citation

If you find POLARIS or the DSPI framework useful in your research, please cite:

Sun, Y., Dai, C., Lu, R., Ji, S., Su, Y., Yu, A., 2026. POLARIS: A sub-meter RGB--NIR benchmark with dual-stage spectral-prior injection for joint ice--snow--water mapping in inhabited circumpolar regions. _ISPRS Journal of Photogrammetry and Remote Sensing_, under review.

You can also use the following BibTeX entry:

```bibtex
@article{polaris_dspi_isprs2026,
  title   = {POLARIS: A sub-meter RGB--NIR benchmark with dual-stage spectral-prior injection for joint ice--snow--water mapping in inhabited circumpolar regions},
  author  = {Sun, Yongqi and Dai, Chenguang and Lu, Ruihua and Ji, Song and Su, Yu and Yu, Anzhu},
  journal = {ISPRS Journal of Photogrammetry and Remote Sensing},
  year    = {2026},
  note    = {under review}
}
```

---

## Contact

For questions about the dataset or code, please contact:

- Yongqi Sun: `sunyq2002@163.com`
- Anzhu Yu (corresponding author): `anzhu_yu@126.com`
