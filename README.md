# PINNeikonal
Eikonal solution using physics-informed neural networks

The eikonal equation is utilized across a wide spectrum of science and engineering disciplines. In seismology, it regulates seismic wave traveltimes needed for applications like source localization, imaging, and inversion. Several numerical algorithms have been developed over the years to solve the eikonal equation. However, they suffer from computational bottleneck when repeated computations are needed for perturbations in the velocity model and/or the source location, particularly in large 3D models. Here, we develop a novel algorithm to solve the eikonal equation based on the emerging paradigm of physics-informed neural networks (PINNs). By minimizing a loss function formed by imposing the eikonal equation, we train a neural network to output traveltimes that are consistent with the underlying partial differential equation. More specifically, to tackle point-source singularity, we use the factored eikonal equation. We observe sufficiently high traveltime accuracy for most applications of interest. We also demonstrate how the proposed algorithm harnesses machine learning techniques like transfer learning and surrogate modeling to massively speed up traveltime computations for updated velocity models and source locations. These properties of the proposed PINN eikonal solver are highly desirable in obtaining an efficient forward modeling engine for seismic inversion applications.

## Libraries
The scripts work with Tensorflow v2.2.0, Keras v2.3.1, and SciAnn v0.4.6.2


## Citation
If you find our work useful in your research, please cite:
```
@article{waheed2020eikonal,
  title={Eikonal solution using physics-informed neural networks},
  author={Waheed, Umair bin and Haghighat, Ehsan and Alkhalifah, Tariq and Song, Chao and Hao, Qi},
  journal={arXiv preprint arXiv:2007.08330},
  year={2020}
}
```

## Contact
If you have any questions, please feel free to email the author.
