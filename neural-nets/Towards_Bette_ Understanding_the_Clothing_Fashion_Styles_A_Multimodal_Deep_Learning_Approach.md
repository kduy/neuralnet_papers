# Paper

* **Title**: owards Better Understanding the Clothing Fashion Styles: A Multimodal Deep Learning Approach
* **Authors**: Yihui Ma1, Jia Jia1∗, Suping Zhou3, Jingtian Fu12, Yejun Liu12 and Zijian Tong4
* **Link**: http://hcsi.cs.tsinghua.edu.cn/static/Paper/Paper17/AAAI17-YIHUI.pdf

# Summary
**Contribution**
  * They construct a benchmark clothing fashion dataset containing 32133 full-body fashion show images from Vogue in the last 10 years. The collected dataset is labeled with complete visual features.
  * They build a universal Fashion Semantic Space (FSS) to describe clothing fashion styles quantitatively. It is a twodimensional image-scale space containing hundreds of words that people often use to describe clothing on shopping websites. Based on the FSS, we can not only do quantitative evaluation on fashion collocation, but also analyze the dynamic change of fashion trends intuitively.
  * They propose a fashion-oriented multimodal deep learning based model, Bimodal Correlative Deep Autoencoder (BCDA), connected with regression to implement the task of mapping visual features to FSS (?)

**How**

*Building the fashion senmatic space*
    + Keywords: Kobayashi proposed 180 keywords in 16 aesthetic categories and defined their coordinate values in the image-scale space (Kobayashi 1995)
    + Fashion styles aesthetic words:
      + Obeserve all the comments from the colthing section of Amazon and split them by words
      + Retained only adjective words (Using WordNet (Miller 1995))
      + Remove words which are not often used to describe clothing (such as: happy, sad, ...) -> 527 aesthetic words representing fashion styles
    + To determine the coordinates of these keywords, they calculate the senmantic distances between keywords and asthetic words using WordNet::Similarity (Pedersen, Patwardhan, and Michelizzi 2004). For an word to be coordinated, they choose 3 keywords with the shortest distances, 
*Fashion-Oriented Multimodal Deep Learning Based BCDA (?)*
   
      
# Dataset
 * Collect 32133 full-body fashion show images in the last 10 years downloaded from Vogue.
 * Annotation details of our dataset:
   * Clothing visual features:
     + Define the visual features of clothing from 2 aspects:
       - color features: Extract 5 color theme of clothing images adopting the algorithm proposed by (Wang et al. 2013).
       - pattern features: annotate images 
     + Fashion style feature: 
       * For annotation of fashion styles: They provide the FSS space for the annotators, who are well trained with the annotation method. For each image:
         - Choose style section in FFS 
         - Determine a specific coordinate for the image according to the distribution of fashion style words
       * For coordinates in the FSS
         - warm-cool and soft-hard coordinates values [-1,1] and he granularity of each dimension is 0.001
         - using the average results of annotators for each image.
 
# Source:


# Related Work
  * Clothing Parsing: 
  * Clothing recommendation:
  * Fashion style modeling:

 


