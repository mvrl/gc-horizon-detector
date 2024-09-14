# Detecting Vanishing Points Using Global Image Context in a Non-Manhattan World

This repo contains the source code of the paper, [Detecting Vanishing Points using Global Image Context in a Non-Manhattan World](http://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Zhai_Detecting_Vanishing_Points_CVPR_2016_paper.pdf).

## Abstract

We propose a novel method for detecting horizontal vanishing points and the zenith vanishing point in man-made environments. The dominant trend in existing methods is to first find candidate vanishing points, then remove outliers by enforcing mutual orthogonality. Our method reverses this process: we propose a set of horizon line candidates and score each based on the vanishing points it contains. A key element of our approach is the use of global image context, extracted with a deep convolutional network, to constrain the set of candidates under consideration. Our method does not make a Manhattan-world assumption and can operate effectively on scenes with only a single horizontal vanishing point. We evaluate our approach on three benchmark datasets and achieve state-of-the-art performance on each. In addition, our approach is significantly faster than the previous best method.

[[Poster](https://github.com/user-attachments/files/17003180/fasthor-poster.pdf)] [[Slides](https://github.com/user-attachments/files/17003181/fasthor-slides.pdf)]

![cover](https://github.com/user-attachments/assets/c6e2d6ad-a59f-457d-b172-120c7ead1e5a)


## Installation:
  1. Install Caffe and compile Matcaffe (see toturial at [Caffe Installation](http://caffe.berkeleyvision.org/installation.html)).
  2. Download the [Caffe model](https://wustl.box.com/v/deephorizonshare), and uncompress the tarball to "assets".
  3. Compile LSD (Line Segment Detector):

  ```bash
  $ cd assets/lsd; make
  ```

## Note:

We recently updated our CNN model to a state-of-the-art network, which is trained with the approach introduced by another excellent work: [Horizon Lines in the Wild](https://www.scottworkman.com/research/deephorizon/).

If you require the original implementation of our work, you can still check the old version:

```bash
$ git checkout v1.0
```

## Citation

Zhai, M., Workman, S., & Jacobs, N. (2016). Detecting Vanishing Points using Global Image Context in a Non-Manhattan World. In IEEE Conference on Computer Vision and Pattern Recognition (CVPR).

Bibtex: 
```
@inproceedings{zhai2016horizon,
  author = {Zhai, Menghua and Workman, Scott and Jacobs, Nathan},
  booktitle = {IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
  title = {Detecting Vanishing Points using Global Image Context in a Non-{Manhattan} World},
  doi = {10.1109/CVPR.2016.610},
  year = {2016}
}
```
