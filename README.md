# Image_search_UserText
Image Search on Large Driving Perception dataset using User Input Text

This repository consists of following two Jupyter notebooks: 

1. Create_Embeddings_fromImageDataset.ipynb
    Creates Vector Embeddings using the Images from the Large Autonomous driving Perception Dataset- ONE MILLION SCENES: ONCE Dataset [decord]https://once-for-auto-driving.github.io/index.html
    Embeddings are created using BLIP[decord]https://github.com/salesforce/BLIP/blob/main/demo.ipynb
3. Search_ImageEmbeddings_fromUserText.ipynb
     Search the Images semantically similar to the User Text leveraging the Vector embeddings created in Step 1.


### Citation
<pre>
@article{mao2021one,
  title={One Million Scenes for Autonomous Driving: ONCE Dataset},
  author={Mao, Jiageng and Niu, Minzhe and Jiang, Chenhan and Liang, Hanxue and Liang, Xiaodan and Li, Yamin and Ye, Chaoqiang and Zhang, Wei and Li, Zhenguo and Yu, Jie and others},
  journal={NeurIPS},
  year={2021}
}
@inproceedings{li2022blip,
      title={BLIP: Bootstrapping Language-Image Pre-training for Unified Vision-Language Understanding and Generation}, 
      author={Junnan Li and Dongxu Li and Caiming Xiong and Steven Hoi},
      year={2022},
      booktitle={ICML},
}<pre>
