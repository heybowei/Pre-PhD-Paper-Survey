# RF Sensing-enabled Interference Mitigation for Wi-Fi-based IoT Systems: A Deep Learning Approach

[Paper Link](https://ieeexplore.ieee.org/abstract/document/10735625?casa_token=HjrbfyTAdyQAAAAA:1Ij7dW95EWOdVzusRY7eV3NHc_6v73yxl4y04WOE-Kz0EQYJJxMDw99BrMW6PT43Pn99ua13Ww>)

## STAR Principle

**Situation:** Blue Tooth and Zig Bee uses the same band, having interference.

**Task:** The location of router can make a difference on throughput. That is to find the best location of router to improve throughput.

**Actions:**

1. The data collect: how to collect a big enough dataset to train a model? (Using GAN to generate data) A way to generate confident data.
2. Mapping CSI to Location. (we can train a model using ground truth and predict the generated data) A common method.
3. Find the relationship between CSI and throughput (use one class SVM to filter out the impossible CSI and use them to calculate the rate of package loss to get throughput) One-class SVM can be used to filter the abnormal data. It apply PCA first and then OCSVM.


## How does this paper can be used to me

1. The GAN model to generate data part is interesting, especially in the RF samples domain. RF samples are difficult to capture and labeled compared to the data amount needed in deep learning.

2. One-Class SVM is a useful tool to distinguish abnormal date when only have positive samples.

3. Simple mapping method: CSI -> predicted package loss -> Throughput. (It can only roughly calculate throughput)