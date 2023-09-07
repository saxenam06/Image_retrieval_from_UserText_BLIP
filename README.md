![image](https://github.com/saxenam06/Image_search_UserText/assets/83720464/d0bb012d-8fb7-499f-b5b9-c30fcc2cb33b)# Image_search_UserText
Image Search on Large Driving Perception dataset using an User Input Text

This repository consists of following two Jupyter notebooks: 

1. Create_Embeddings_fromImageDataset.ipynb
    - Creates Vector Embeddings using the Images from the Large Autonomous driving Perception Dataset- ONE MILLION SCENES:  [ONCE Dataset](https://once-for-auto-driving.github.io/index.html). 
    - Embeddings are created using [BLIP](https://github.com/salesforce/BLIP/blob/main/demo.ipynb).
2. Search_ImageEmbeddings_fromUserText.ipynb
     - Search the Images semantically similar to the Input User Text leveraging the Vector embeddings created in Step 1.
     - Search or Image-Text Matching is also done using [BLIP](https://github.com/salesforce/BLIP/blob/main/demo.ipynb).
     - Top 3 images matching the example user Text "a car driving on an intersection" are given in the notebook and are shown below. 
        ![image](https://github.com/saxenam06/Image_search_UserText/assets/83720464/a2749738-bf75-4bdc-8896-ce1907884849)

3. Pyspark is used to read the large Image dataset in a Spark Dataframe and then perform Distributed Inferece (Calculation of Embeddings and Image-Text Matching Scores using the Pretrained model).

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
