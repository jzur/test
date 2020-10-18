# test

**timethod** is a Matlab package for computing all zeros of harmonic mapping by continuation.

---

## Installation

To clone the timethod repository, first navigate in a terminal to where you want the repository cloned, then type
```
git clone TODO
```
To use timethod in Matlab, you will need to add the `timethod` directory to the Matlab path.

---

## Basic usage

To compute all zeros of the harmonic mapping

![formula](https://render.githubusercontent.com/render/math?math=f(z)=z^2)

we type:

```matlab
fun = harmonicRat([1 0 0], [1], [2 1], [1 1 0], [1], [0]);
zer = tiroots_rand(fun)
res = max(abs(fun.f(zer)))
```
Output:

```matlab
zer =
  -0.8775 - 0.9278i
  -0.8775 + 0.9278i
  -1.4569 + 0.0000i
  -0.5872 - 0.0000i
res =
   8.8818e-16
```

For more examples we refer to the experiments in ex_*.m.


## Citing timethod

If you find timethod useful in your work, we kindly request that you cite the [following preprint](https://arxiv.org/abs/xxyyzz):

```latex
@article{SeteZur2020,
	Author = {S\`{e}te, Olivier \and Zur, Jan},
	Journal = {ArXiv e-prints: xxyyzz},
	Title = {{The transport of images method: computing all zeros of harmonic mappings by continuation}},
	Url = {https://arxiv.org/abs/xxyyzz.pdf},
	Year = {2020},
}
```

