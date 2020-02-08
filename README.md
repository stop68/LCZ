# Local Climate Zone Mapping as Remote Sensing Scene Classification using Deep Learning: A Case Study of Metropolitan China

Contact: liusj@hku.hk or sjliu.me@gmail.com


## Training and Testing Data
[Download Training and Testing Data Here](https://sjliu.me/lcz/data/lcz_sample_shp_release.zip)

| Region  | Major City  | Note  |  
|---|---|---|
|  The Greater Bay Area |  Guangzhou, Shenzhen, Zhuhai, Macau and Hong Kong | Part of Zhongshan, Jiangmen, Dongguan, Huizhou and Foshan are included  |   
| The Shanghai Metropolis  | Shanghai and Hangzhou  |  Part of Shaoxing and Jiaxing are included |  
| The Beijing Metropolis  |  Beijing and Tianjin |  Part of Tangshan are included |  


## Pretrained model
[Download Pretrained Model Here](https://sjliu.me/lcz)

The size of input is <img src="https://render.githubusercontent.com/render/math?math=64\times 64"> with 10 channels

```
The channel order is (channel & Sentinel-2 band):
[0,1,2,3,4,5,6, 7, 8, 9] = [2,3,4,5,6,7,8,11,12,8A]
```



Please use the follow normalization when applying the model.
```
data = data/5000.0
data = np.float32(data)
```




