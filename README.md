# CS4243 Project
Fast Image Vector Search Tool built in PyTorch

# Set-up Datasets
1. Download datasets: [QuickDraw](https://console.cloud.google.com/storage/browser/quickdraw_dataset/full/numpy_bitmap), [Sketchy](https://tinyurl.com/v2dj69y9), [TUBerlin](http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/sketches_png.zip).
2. Unzip datasets QuickDraw, Sketchy and TUBerlin in `dataset/`, rename into `quickdraw/`, `sketchy/` and `tuberlin/` respectively, unzip TUBerlin's [info.txt](https://tinyurl.com/yxv6s8dv) in `dataset/sketchy/`.
3. Run [dataset.ipynb](dataset.ipynb).

# Dataset
- CIFAR10
    - ![image](https://user-images.githubusercontent.com/27071473/158947211-5c05aab3-4d7c-424f-94c1-423bcf32cb7a.png)
    - Image shape: (32, 32, 3)
    - No. classes: 9
    - Classes: airplane, car, bird, cat, dog, frog, horse, ship, truck
    - Count per class (train/test):
        - airplane - 5000/1000
        - car - 5000/1000
        - bird - 5000/1000
        - cat - 5000/1000
        - dog - 5000/1000
        - frog - 5000/1000
        - horse - 5000/1000
        - ship - 5000/1000
        - truck - 5000/1000
    - Dataset size (train/test): 45000/9000
    - Download - Run `download-cifar.ipynb`, then run `dataset.ipynb`.
    - [Website](https://www.cs.toronto.edu/~kriz/cifar.html)
- QuickDraw
    - ![image](https://user-images.githubusercontent.com/27071473/158947246-b1d168c0-2108-4ed5-9e57-8330e3faa5b7.png)
    - Image shape: (28, 28)
    - No. classes: 9
    - Classes: airplane, bird, car, cat, ship, dog, frog, horse, truck
    - Count per class:
        - airplane - 151623
        - bird - 133572
        - car - 182764
        - cat - 123202
        - ship - 123410
        - dog - 152159
        - frog - 159047
        - horse - 178286
        - truck - 131354
    - Dataset size: 1335417
    - [Code](https://github.com/googlecreativelab/quickdraw-dataset)
    - [Dataset (Numpy 28x28 grayscale bitmap .npy)](https://console.cloud.google.com/storage/browser/quickdraw_dataset/full/numpy_bitmap)
- Sketchy
    - ![image](https://user-images.githubusercontent.com/27071473/158947274-707285cf-6175-4ad9-9726-27d7db93f6d7.png)
    - ![image](https://user-images.githubusercontent.com/27071473/158958660-522b8a08-c2b0-407e-830a-6e5cadd63cb8.png)
    - Real
        - Image shape: (256, 256, 3)
        - No. classes: 8
        - Classes: airplane, car, cat, dog, frog, horse, truck, bird
        - Count per class:
            - airplane - 100
            - car - 100
            - cat - 100
            - dog - 100
            - frog - 100
            - horse - 100
            - truck - 100
            - bird - 100
        - Dataset size: 800
    - Doodle
        - Image shape: (256, 256)
        - No. classes: 8
        - Classes: airplane, car, cat, dog, frog, horse, truck, bird
        - Count per class:
            - airplane - 528
            - car - 534
            - cat - 512
            - dog - 512
            - frog - 502
            - horse - 525
            - truck - 524
            - bird - 504
    - Dataset size: 4141
    - [Paper](https://sketchy.eye.gatech.edu/paper.pdf)
    - [Website](https://sketchy.eye.gatech.edu/)
    - [Code](https://github.com/CDOTAD/SketchyDatabase)
    - [Dataset (Sketches and Photos)](https://tinyurl.com/v2dj69y9)
    - [Supplementary Report](https://sketchy.eye.gatech.edu/supp.pdf)
- TUBerlin
    - ![image](https://user-images.githubusercontent.com/27071473/158947259-692a5110-3e49-43db-8bb6-05778c6ef01c.png)
    - Image shape: (1111, 1111)
    - No. classes: 8
    - Classes: airplane, car, cat, dog, bird, frog, horse, truck
    - Count per class:
        - airplane - 80
        - car - 80
        - cat - 80
        - dog - 80
        - bird - 80
        - frog - 80
        - horse - 80
        - truck - 80
    - Dataset size: 640
    - [Paper](http://cybertron.cg.tu-berlin.de/eitz/pdf/2012_siggraph_classifysketch.pdf)
    - [Website](http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/)
    - [Dataset (Sketches in png)](http://cybertron.cg.tu-berlin.de/eitz/projects/classifysketch/sketches_png.zip)
