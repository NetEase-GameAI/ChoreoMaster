 # "ChoreoMaster: Choreography -Oriented Music Driven Dance Synthesis"
## 1. Description

 To facilitate further research in this area, we release the copyright-free portion of our paired music/motion [dataset](https://drive.google.com/file/d/1R5MYYy4PSkLoifFzmCwPn9dBp8DVshxV/view?usp=sharing) (1.48 hours out of 9.91 hours).  It contains 2708 dance motion meters (the motion unit used to construct motion graph), all paired with music clips and labels, with a total frame count of 160136 sampled at 30 fps.

The motion, music and label files are respectively stored in three folders ("label_json", "motion_fbx", "music_clip") with the same prefix name. All the motion files are saved as .fbx format and we also provide a T-pos model file.

This dataset can only be used for the sole purpose of performing **non-commercial scientific research**. Any other use, in particular any use for commercial purposes, is prohibited.


## 2. Label Format:
The label file are saved as json format, containing the two dimentional music and motion styles and the corresponding rhythm signature.

```
{
    "name": the motion clip name with the format of motion_id@clip_id,  consecutive clips will have the same motion_id with consecutive clip_id
    "music_style1": music style 1,
    "music_style2": music style 2,
    "motion_style1": motion style 1,
    "motion_style2": motion style 2,
    "signature": 8 bit rhythm signature string
}
```

Details about the style labels and rhythm signatures can be found in our paper. 


## 3. Publications:
If you use our dataset in your work, please cite our article:

```
@article{choreomaster2021,
    author = {Chen Kang, Zhipeng Tan, Jin Lei, Song-Hai Zhang, Yuan-Chen Guo, Weidong Zhang, Shi-Min Hu},
    title = {ChoreoMaster : Choreography-Oriented Music-Driven Dance Synthesis},
    journal = {ACM Transactions on Graphics (TOG)},
    volume = {40},
    number = {4},
    year = {2021},
    publisher = {ACM}
  }
```
