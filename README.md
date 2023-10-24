<br />
<div align="center">
  <a href="https://ship-ai.ikim.nrw/">
    <img src="images/boa-logo.svg" alt="Logo">
  </a>
</div>

# BOA: Body and Organ Analysis

## What is it?
BOA is a tool for segmentation of CT scans developed by the [SHIP-AI group at the Institute for Artificial Intelligence in Medicine](https://ship-ai.ikim.nrw/). Combining the [TotalSegmentator](https://arxiv.org/abs/2208.05868) and the [Body Composition Analysis](https://pubmed.ncbi.nlm.nih.gov/32945971/), this tool is capable of analyzing medical images and identifying the different structures within the human body, including bones, muscles, organs, and blood vessels.


If you use this tool, please cite the following papers:

```
Haubold J, Baldini G, Parmar V, et al. A CT-Based Body and Organ Analysis for Radiologists at the Point of Care. Invest. Radiol. (In Press).
```

```
Wasserthal J, Breit H-C, Meyer MT, et al. TotalSegmentator: Robust Segmentation of 104 Anatomic Structures in CT Images. Radiol. Artif. Intell. 2023:e230024. Available at: https://pubs.rsna.org/doi/10.1148/ryai.230024.
```

```
Isensee F, Jaeger PF, Kohl SAA, et al. nnU-Net: a self-configuring method for deep learning-based biomedical image segmentation. Nat. Methods. 2021;18(2):203–211. Available at: https://www.nature.com/articles/s41592-020-01008-z.
```

## How to run?

* Set up the [environment variables](./documentation/environment_variables.md).
* Either use the [PACS integration](./documentation/pacs_integration.md) or the [command line tool](./documentation/command_line_tool.md).

### Notes on Performance

To make an estimate on how much power and time is needed to process a study, we used the [following table](https://github.com/wasserth/TotalSegmentator/blob/master/resources/imgs/runtime_table.png) provided by the TotalSegmentator. However, for very large series (e.g. 1600 slices 1mm), the performance may be worse and more CPU power may be needed. According to our tests, 16GB of GPU should be sufficient.
