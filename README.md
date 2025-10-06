# BSD10k (Broad Sound Dataset 10k)

The **BSD10k dataset** (Broad Sound Dataset 10k) is an open collection of human-labeled sounds containing over 10k [Freesound](https://freesound.org/) audio clips, annotated according to the 23 second-level classes defined in the Broad Sound Taxonomy. The dataset has been created at the [Music Technology Group](https://www.upf.edu/web/mtg) of Universitat Pompeu Fabra.

## Dataset characteristics
The dataset comprises heterogeneous sounds from [Freesound](https://freesound.org/). 
The sounds are cropped to a maximum length of 30 seconds, resulting in variable durations ranging from 0.01 to 30s. 
Audio lengths vary due to the heterogeneity of the sound classes and the range of contributions from Freesound users. 
The original files downloaded from Freesound are converted to a standardized format of uncompressed WAV files with 44.1 kHz sampling rate, 16-bit depth, and mono channel. 
All sounds have been manually labeled by human annotators. 
BSD10k categorizes the sounds into 23 classes, which are the second-level categories of the Broad Sound Taxonomy (see details below). The annotated data has a non-uniform distribution across these categories. 
The dataset and its respective versions are available in the [Zenodo archive](https://zenodo.org/records/17233905).
For each audio file, the **latest version** of the dataset includes the following: the `category label` assigned during annotation and its `confidence score`, descriptive metadata (`title`, `tags`, `description`), and provenance information (`ID`, `uploader`, `license`).
We also provide precomputed embeddings to facilitate further analysis and reproducibility.
For more details on the dataset creation and its contents, please refer to our paper "*Heterogeneous Sound Classification with the Broad Sound Taxonomy and Dataset*" (Section 3.1).
The second version of the dataset is first presented in "*Hierarchical and Multimodal Learning for Heterogeneous Sound Classification*".

## Versioning 
### v1.1 – 2025-10-02
- Sound count: 10,956
- Total hours: 35.25
- Metadata fields: ID, class (code, index, top level), confidence, title, tags, description, uploader, license
- Features (precomputed): CLAP audio embeddings, CLAP text embeddings
- Notes: Added description, confidence score, precomputed embeddings
  
### v1.0 – 2024-07-11
- Sound count: 10,309
- Total hours: 32.5
- Metadata fields: ID, class (code, index, top level), title, tags, uploader, license
- Notes: Initial version

## Taxonomy
The **Broad Sound Taxonomy (BST)** organizes sounds into a two-level hierarchical structure with 5 top-level and 23 second-level classes. 
The top-level categories cover distinct types of sounds: *Music*, *Instrument samples*, *Speech*, *Sound effects*, and *Soundscapes*. 
The taxonomy is designed to classify *any type* of sound while remaining broad, comprehensive, and easy to use. It can be used for *organizing and filtering sounds* in heterogeneous sound collections, such as Freesound, as well as in personal sound libraries. 
Additional information about the taxonomy, including its design principles, detailed taxonomy creation methodology and evaluation, is provided in the journal article "*A General-Purpose Sound Taxonomy for the Classification of Heterogeneous Sound Collections*".

<img src="BST_diagram.png" style="width:85%; height:auto;">

## Data
The audio files and metadata of the dataset can be downloaded from Zenodo: **[Access BSD10k data](https://zenodo.org/records/17233905)**

## Baseline
[TODO]

## Cite us 


If you use this dataset, please cite our papers:

<a href="https://arxiv.org/pdf/2410.00980"><img src="https://img.shields.io/badge/download-PDF-green.svg" alt="View BSD10K v1.0 paper in PDF format" title="View BSD10K v1.0 paper in PDF format" align="right" /></a>
**BSD10k v1.0** 
> Anastasopoulou, P., Torrey, J., Serra, X., & Font, F. (2024). Heterogeneous sound classification with the Broad Sound Taxonomy and Dataset. In Proc. Workshop on Detection and Classification of Acoustic Scenes and Events (DCASE).

<a href="https://dcase.community/documents/workshop2025/proceedings/DCASE2025Workshop_Anastasopoulou_35.pdf"><img src="https://img.shields.io/badge/download-PDF-green.svg" alt="View BSD10K v1.1 paper in PDF format" title="View BSD10K v1.1 paper in PDF format" align="right" /></a>
**BSD10k v1.1** 
> Anastasopoulou, P., Dal Ri, F., Serra, X., & Font, F. (2025). Hierarchical and multimodal learning for heterogeneous sound classification. In Proc. Workshop on Detection and Classification of Acoustic Scenes and Events (DCASE).

## License
BSD10k is released in its entirety under the [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/). 
We note, though, that each audio file is released under its own Creative Commons (CC) license, as defined by the uploader in Freesound. 
Some sounds require attribution to their original authors, while others forbid commercial reuse. 
If the dataset is used in a commercial setting, the sounds with CC-BY-NC licenses should be excluded.
Links to the *license deeds* for each sound can be further accessed through the `metadata` files of each version.
