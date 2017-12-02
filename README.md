# tsne-grid
This is a python script for [tsne](https://lvdmaaten.github.io/tsne/) visualization of multiple images in a square grid.

<!-- ![alt text](./examples/outputs/output5x5.jpg =250x250) -->
<p align="center">
<img src="./examples/outputs/output5x5.jpg" width="300" height="300" />
<img src="./examples/outputs/output8x8.jpg" width="300" height="300" />

</p>

### Setup
Dependencies:
* [tensorflow](https://www.tensorflow.org/install/)
* [keras](https://keras.io/)

### Usage

Basic usage:
```bash
python tsne_grid.py --dir ./examples/inputs/ --size 4
```
#### Options (required)
* `--dir`: Input images directory containing image collection.
* `--size`: Number of small images in a row/column in output image.

#### Options (optional)
* `--res`: Width/height if small images (in pixels). Default is 224.
* `--name`: Output filename. Default is tsne_grid.jpg
* `--path`: Output image path. Default is current directory.
* `--per`: Perplexity for tsne algorithm. Default is 50.
* `--iter`: Number of iterations for tsne algorithm. Default is 5000.

