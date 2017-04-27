# Paper

* **Title**: Clothing Co-Parsing by Joint Image Segmentation and Labeling
* **Authors**: Wei Yang1, Ping Luo2, Liang Lin
* **Link**: https://arxiv.org/pdf/1502.00739.pdf

# Summary
* What
  * This paper aims at developing an integrated system of clothing co-parsing, in order to jointly parse a set of clothing images (unsegmented but annotated with tags) into semantic configurations
  * Propose a data-driven framework consisting of two phases of inference:
    + image co-segmentation
    + region co-labeling
  * Achieve 90.29% / 88.23% segmentation accuracy and 65.52% / 63.89% recognition rate on the Fashionista and the CCP dataset
 
 * How
   * They build a system consisting 2 sequential phases of inference over a set of colthing images:
    + image co-segmentation for extracting distinguishable clothes regions
    + region co-labeling for recognizing various garment items
   * Furthermore, they exploit contexts of clothing configuration, e.g., spatial locations and mutual relations of clothes items, inspired by the successes of object/scene context modeling
   
   **Co-segmentation**
    + Extract superpixels and group them into regions for each images. Using MRF model
    + Train a number of E-SVM classifiers for the selected regions using the HOG feature, i.e., one classifier for one region, and produce a set of region-based detectors, as shown in Figure 1 (a3), which are applied as top-down templates to localize similar regions over all images.
   **Co-labeling**
    + They construct a multi-image graphical model by taking the regions as vertices of graph. In this model, they link adjacent regions within each image as well as regions across different images, which shares similar appearance and latent semantic tags.
    + Thus they use statistical strength from similar regions in different images and assign labels jointly. 
    + The optimization of co-labeling is solved by the efficient Graph Cuts algorith
   
# Dataset
 Fashionista: https://github.com/grahamar/fashion_dataset
 CCP: https://github.com/bearpaw/clothing-co-parsing
 
# Source 


# Related Work

 


