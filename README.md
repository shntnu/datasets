# JUMP Cell Painting Datasets

This is a collection of [Cell Painting](https://jump-cellpainting.broadinstitute.org/cell-painting) image datasets generated by the [JUMP-CP Consortium](https://jump-cellpainting.broadinstitute.org/).

This repository contains notebooks and instructions to work with the datasets.

All the data is hosted on the Cell Painting Gallery on the Registry of Open Data on AWS ([https://registry.opendata.aws/cellpainting-gallery/](https://registry.opendata.aws/cellpainting-gallery/)).

## Details about the data

Currently, this collection comprises 5 datasets:

- The principal dataset of 116k chemical and >15k genetic perturbations the partners created in tandem (`cpg0016`), split across 12 data-generating centers (“sources”).
- 3 pilot datasets created to test: different perturbation conditions (`cpg0000`), staining conditions (`cpg0001`), and microscopes (`cpg0002`).
- A previously-published dataset of 30k chemical perturbations reprocessed to make it compatible with the rest of the JUMP datasets (`cpg0012`).

### What’s available now

- All data [components](https://github.com/broadinstitute/cellpainting-gallery/blob/main/folder_structure.md) of the three pilots and the reprocessed dataset.
- Most data components (images, raw CellProfiler output, single-cell profiles, aggregated CellProfiler profiles) from 6 sources for the principal dataset.
- The first draft of a map for all the wells currently available in the principal dataset. The file maps each well to a unique perturbation id (`jcp2022_id`).
- The first draft of a metadata file that maps each `jcp2022_id` to available metadata about the perturbation.
- A notebook to load and inspect the data currently available in the principal dataset.

**Please note: At present in the principal dataset (`cpg0016`), many compounds will be missing replicates, and a full QC of the dataset is pending. We don’t recommend performing any analysis with the principal dataset until all the remaining components and all sources are uploaded and the full QC of the dataset is complete. The other datasets are complete.**

### What’s coming up

- Extending the map and metadata and notebooks to the three pilots and the reprocessed dataset so that all these datasets can be quickly loaded together.
- Curated annotations for the compounds, obtained from [ChemBL](https://www.ebi.ac.uk/chembl/) and other sources.
- The remaining data [components](https://github.com/broadinstitute/cellpainting-gallery/blob/main/folder_structure.md) (normalized profiles, feature selected profiles, treatment-level consensus profiles, quality control results) and the remaining sources for the principal dataset.
- Deep learning [embeddings](https://tfhub.dev/google/imagenet/efficientnet_v2_imagenet1k_s/feature_vector/2) using a pre-trained neural network for all 5 datasets.
- [Quality control](https://github.com/broadinstitute/cellpainting-gallery/blob/main/folder_structure.md#quality_control-folder-structure) results at the image level for the principal dataset to allow removing bad images.
- Our manuscript, Chandrasekaran et al., 2022b, which is being approved by pharmaceutical company partners and will be released on bioRxiv.

## Statistics

TODO

## How to load the data: notebooks

TODO: See notebook [URL] to learn more about how to load the data in the principal dataset.

## Citation/license

### Citing the JUMP resource as a whole

All the data is released with CC0 1.0 Universal (CC0 1.0). 
Still, professional ethics require that you cite the associated publication. 
Please use the following format to cite this resource as a whole:

_We used the JUMP Cell Painting datasets (Chandrasekaran et al., 2022b), available from the Cell Painting Gallery on the Registry of Open Data on AWS ([https://registry.opendata.aws/cellpainting-gallery/](https://registry.opendata.aws/cellpainting-gallery/))._

Please note that the JUMP whole-project manuscript (Chandrasekaran et al., 2022b) is currently in preparation.

### Citing individual JUMP datasets

To cite individual JUMP Cell Painting datasets, please follow the guidelines in the Cell Painting Gallery citation [guide](https://github.com/broadinstitute/cellpainting-gallery/#citationlicense). 
Examples are as follows:

_We used the dataset cpg001 (Cimini et al., 2022), available from the Cell Painting Gallery on the Registry of Open Data on AWS (https://registry.opendata.aws/cellpainting-gallery/)._

_We used the dataset cpg000 (Chandrasekaran et al., 2022a), available from the Cell Painting Gallery on the Registry of Open Data on AWS (https://registry.opendata.aws/cellpainting-gallery/)._

## Questions?

Please ask your questions via issues [https://github.com/jump-cellpainting/datasets/issues](https://github.com/jump-cellpainting/dataset/issues).