# Image_search_UserText
Image Search on Large Driving Perception dataset using an User Input Text

This repository consists of following two Jupyter notebooks: 

1. Create_Embeddings_fromImageDataset.ipynb
    - Creates Vector Embeddings using the Images from the Large Autonomous driving Perception Dataset- ONE MILLION SCENES:  [ONCE Dataset](https://once-for-auto-driving.github.io/index.html). 
    - Vector Embeddings are created using [BLIP](https://github.com/salesforce/BLIP/blob/main/demo.ipynb) and are stored for Step 2.
2. Retrieve_Image_from_UserText.ipynb
     - Search the Vector Embeddings corresponding to Images semantically similar to the Input User Text.
     - Search or Image-Text Matching is also done using [BLIP](https://github.com/salesforce/BLIP/blob/main/demo.ipynb).
     - Top 3 images matching the example user Text _"a car driving on an intersection"_ are given in the notebook and are shown below. 
        ![image](https://github.com/saxenam06/Image_search_UserText/assets/83720464/a2749738-bf75-4bdc-8896-ce1907884849)
       Another example with user text _"a car driving on a highway"_ is shown below. It retrieves images semantically similar to the highway.
       ![image](https://github.com/saxenam06/Image_search_UserText_BLIP/assets/83720464/506fa890-a027-4af5-bf0d-5cda26d7f483)

        ![image](https://github.com/saxenam06/Image_search_UserText_BLIP/assets/83720464/ba043833-1f28-4f8c-9902-e657374afab4)
     You can try More!!
3. Pyspark is used to read the large Image dataset in a Spark Dataframe and then perform Distributed Inferece (Calculation of Embeddings and Image-Text Matching Scores using the Pretrained model).

Following Datasets and Models were used in this work.
### References
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
