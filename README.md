# DejaVu
English-Japanese caption dataset including word sense ambiguity for evaluation of multimodal machine translation.

## Dataset Overview

- **Captions**: English captions and their Japanese translations, including 500 target words and 6 different caption templates. All target words have multiple word senses and are designed such that the limited contextual information in the captions is not sufficient to select the correct word sense. In order to translate correctly into Japanese, it is necessary to refer to the corresponding images.
- **Images**: 500 images referenced during translation. These images are obtained from [ImageNet](https://www.image-net.org/update-mar-11-2021.php) and [Flickr](https://www.flickr.com/). The [WordNet](https://wordnet.princeton.edu/) id corresponding to the target word in the caption is used as the image file name.
- **Format**: Images are stored in the `images/` directory, and captions are available in the `captions/` directory. `index.txt` is used to map the id of images in the order of captions.

## Dataset Structure

The dataset is structured as follows:

```
- dataset/
  - images/
      - 10055410.jpg
      - 10149867.jpg
      - ...
  - index.txt
  - captions/
    - en/
      - template1.en
      - template2.en
      - ...
    - ja/
      - template1-1.ja
      - template1-2.ja
      - ...
- README.md
```

## Usage

**Clone the repository**:
 ```bash
 git clone git@github.com:tmu-nlp/DejaVu.git
 ```

## License

This dataset is made available under the [Creative Commons Attribution-ShareAlike (CC BY-SA) license](https://creativecommons.org/licenses/by-sa/4.0/legalcode).

## Citation

If you use this dataset in your research, please cite it as follows:

```
@misc{DejaVu,
  author = {Ayako Sato},
  title = {DejaVu},
  year = {2024},
  howpublished = {\url{https://github.com/tmu-nlp/DejaVu}}
}
```
