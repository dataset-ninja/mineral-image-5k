The authors of the **MineralImage5k** dataset make a significant contribution by introducing an open benchmark for zero-shot raw mineral visual recognition. The dataset consits of more than 5 thousand mineral species, covering almost the span of existing minerals on the Earth. Beyond the zero-shot classification dataset, subsets are provided for segmentation, mineral size estimation, and few-shot classification. Baseline solutions for these computer vision problems are published, inviting the community to surpass them.

### Importance of Mineral Diagnostics

Nature boasts about 6000 known minerals and their varieties, with only a fraction being rock-forming or of industrial interest. Accurate mineral diagnostics is crucial for geological work, enabling geological mapping and deposit exploration. However, exact mineral identification is a complex and time-consuming task, requiring significant skill and time investment by geologists. The involvement of machine intelligence in visual diagnostics aims to optimize this process, freeing up professional mineralogists' time for more complex tasks and identifying errors in visual diagnostics.

The integration of machine intelligence in mineral diagnostics, particularly in raw samples, holds promising implications. If an algorithm can enable visual diagnostics of minerals at the level of an ordinary geologist, it opens avenues for creating search robots for exploring challenging terrains on Earth and potentially on other planets. The addition of visual diagnostics capabilities complements existing methods like IR spectroscopy and Raman spectroscopy, enhancing the selection of objects for analysis and expanding research possibilities.

## Dataset Collection and preprocessing

For dataset creation, the authors utilized the [Fersman mineralogical museum](http://www.fmm.ru/) image set, one of the largest mineralogical collections globally, containing over 170000 samples of about 5000 mineral species. The dataset provides a diverse and representative view of mineral diversity, offering advantages over other datasets.


<img src="https://github.com/dataset-ninja/mineral-image-5k/assets/78355358/b59f3b5c-f289-42d3-9b8d-e904d2e66116" alt="image" width="800">

The authors implemented a comprehensive image preprocessing pipeline to enhance the dataset's quality and representation. This involved removing uninformative images, handling duplicates, and resizing images to a standardized format. The pipeline also addressed potential issues related to text on images, distinguishing between minerals, reference cubes, and text plates.

### Formation of Multiple Datasets

The filtered and cropped images were used to create multiple datasets, including a zero-shot classification dataset and subsets for few-shot classification. Additionally, auxiliary datasets for segmentation and mineral size estimation were provided, featuring manually labeled mineral and satellite masks and manually measured mineral sizes, respectively.

| Classes | Images | Minimum images per class | Task           | Subsets              |
|---------|--------|--------------------------|----------------|----------------------|
| 5139    | 44784  | 1                      | Classification | Test                 |
| 360     | 31982  | 17                      | Classification | Train&Test           |
| 98      | 23496  | 78                      | Classification | Train&Test           |
| 36      | 16001  | 187                      | Classification | Train&Test           |
| 10      | 8549   | 462                      | Classification | Train&Test           |
| –       | >100   | –                        | Segmentation   | Test                 |
| –       | 18076  | –                     | Regression (size estimation)     | Test |

<span style="font-size: smaller; font-style: italic;">The proposed subsets with different classes definition.</span>
