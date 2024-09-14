## gc-horizon-detector
This repo contains the source code of the paper, [Detecting Vanishing Points using Global Image Context in a Non-Manhattan World](http://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Zhai_Detecting_Vanishing_Points_CVPR_2016_paper.pdf).

### Installation:
  1. Install Caffe and compile Matcaffe (see toturial at [Caffe Installation](http://caffe.berkeleyvision.org/installation.html)).
  2. Download the [Caffe model](https://wustl.box.com/v/deephorizonshare), and uncompress the tarball to "assets".
  3. Compile LSD (Line Segment Detector):

  ```bash
  $ cd assets/lsd; make
  ```

### Note:
We recently updated our CNN model to a state-of-the-art network, which is trained with the approach introduced by another excellent work: [Horizon Lines in the Wild](http://cs.uky.edu/~scott/research/deephorizon/).

If you require the original implementation of our work, you can still check the old version:

```bash
$ git checkout v1.0
```
