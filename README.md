# GeoRic Dataset for Image Captioning
Version 1.0

## Sources

The dataset contains photographs, captions and geographic metadata extracted from [the Geograph project website](https://www.geograph.org.uk/).

## Dataset

### Description

The dataset consists of 29,038 images with the corresponding captions and image location coordinates (latitude and longitude). The captions are naturally produced and contain extensive geographic referencing (mentions of geographic entities in relation to the photograph location).
An example entry in the dataset:

| UUID | URL | Caption | Latitude | Longitude | Split |
| ------------- | ------------- |  :-------------: | :-------------: | :-------------: | :-------------: |
| 709ca41e-c1f3-4ba5-96e2-c49b58f9df8f | https://www.geograph.org.uk/photo/3079623 | Farmland to the west of Burnham Market | 52.93659 | 0.70376 | train |

### Files

- [`georic_dataset_v1.0.csv`](https://drive.google.com/file/d/1fz_zsLG6i0WHTxIiaqso47V4rvrAaAgQ/view?usp=sharing): the GeoRic dataset
- [`georic_images_v1.0.zip`](https://drive.google.com/file/d/10j9x6opvJ1TL9nUbCce5f1dbzQaF50y2/view?usp=sharing): an archived folder with the images from the GeoRic dataset
	- Every image in this folder is extracted from [the Geograph project website](https://www.geograph.org.uk/). All rights to the photographs belong to the original copyright owners.
        - The URLs of the original photographs are provided in the GeoRic dataset.
	- Every image is linked to an entry in the GeoRic dataset by its name:
		- `georic_images/{UUID}.jpg` corresponds to an entry with UUID `UUID`
		- E.g. `georic_images/709ca41e-c1f3-4ba5-96e2-c49b58f9df8f.jpg` corresponds to the example dataset entry above.

## License

The dataset is licensed for reuse under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).

## Disclaimer

The GeoRic dataset is created for research purposes only. We claim no ownership of the photographs in the dataset; the rights to the photographs and all the related materials belong to the original copyright owners.

## Citing GeoRic dataset

Nikiforova, S., Deoskar, T., Paperno, D., and Winter, Y. Geo-Aware Image Caption Generation. To
appear in _Proceedings of the 28th International Conference on Computational Linguistics (COLING
2020)_. 

## Dataset statistics

### Basic statistics

| | Number of captions | Length in tokens | Number of vocabulary words | Number of geo-entities |
| ------ |  :-----------: | :-----------: | :-----------: | :-----------: | 
| **Total** | 29,038 | 289,028 | 229,429 | 59,599 |
| **Average (per caption)** | | 9.95 | 7.9 | 2.05 |

### Spatial prepositions statistics

The number of captions that contain a given spatial preposition.

| | Number of captions |
| ------ |  :-----------: | 
| **Near** | 9602 | 
| **In** | 7090 |
| **Along** | 2359 |
| **Across** | 1776 |
| **North of** | 2233 |
| **South of** | 2058 |
| **East of** | 1267 |
| **West of** | 1374 |
