# ๐ Where's Wally? with U-Net
`Image Segmentation`์ ํตํด Wally์ ์์น๋ฅผ ์ฐพ์๋ด๊ณ ,  
์๋ก์ด ์ด๋ฏธ์ง๊ฐ ๋ค์ด์๋ Wally๋ฅผ ์ฐพ์๋ผ ์ ์๋ `U-Net Model`์ ๊ตฌ์ถํ์์ต๋๋ค.

## 1. DataSet
[ํด๋น ๋งํฌ](https://www.kaggle.com/kairess/find-waldo)์ ๋ฐ์ดํฐ ์์ ์ฌ์ฉํ์ต๋๋ค.  

๋ฐ์ดํฐ ์์ ๋ค์๊ณผ ๊ฐ์ด ๋ถ๋ฅ๋์ด ์์ต๋๋ค.
* imgs_uint8 : ์ ์ฒด ์ด๋ฏธ์ง
* labels_uint8 : wally๊ฐ ์๋ ์์น๋ 1, ๊ทธ ์ธ๋ 0์ผ๋ก ํ์ ๋ ๋ง์คํน ์ด๋ฏธ์ง
* waldo_sub_imgs_uint8 : wally๊ฐ ์๋ ๋ถ๋ถ์ด ํ๋๋ ์ด๋ฏธ์ง
* waldo_sub_labels_uint8 : wally๊ฐ ์๋ ์์น๋ 1, ๊ทธ ์ธ๋ 0์ผ๋ก ํ์ ๋ ํ๋ ๋ง์คํน ์ด๋ฏธ์ง

## 2. Model Structure
<img width="400" alt="image" src="https://user-images.githubusercontent.com/75603262/124211042-6df65600-db27-11eb-9dcb-11dc8cd0aac1.png">  
์ ์ ์์ ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ง๊ณ ๋ ์ ํํ ์ด๋ฏธ์ง ๋ถ๋ฅ๋ฅผ ์ํํ๋ U-Net Model์ ์ฌ์ฉํ์ต๋๋ค.  

[์ด๋ฏธ์ง ์ถ์ฒ](https://medium.com/@msmapark2/u-net-%EB%85%BC%EB%AC%B8-%EB%A6%AC%EB%B7%B0-u-net-convolutional-networks-for-biomedical-image-segmentation-456d6901b28a)

## 3. Demo
<img width="500" alt="demo" src="https://user-images.githubusercontent.com/75603262/124211573-4b187180-db28-11eb-9e7e-14ad13cc475b.png">
๋ชจ๋ธ ํ๊ฐ ๊ฒฐ๊ณผ, 0.99์ ๋์ ์ ํ๋๋ฅผ ํ์ธํ  ์ ์์์ต๋๋ค.  

์๋ก์ด ์ด๋ฏธ์ง๊ฐ ๋ค์ด์์ ๋์๋ ๋ชจ๋ธ์ Wally๋ฅผ ์ฑ๊ณต์ ์ผ๋ก ์ฐพ์๋ด์์ต๋๋ค!

## 4. ํ๋ก์ ํธ ์ ๋ฆฌ
- [ํ๋ก์ ํธ ๋ฐํ ์๋ฃ ๋งํฌ](https://github.com/hyewonsonn/Project4_where-s_wally/blob/main/AI_02_%E1%84%89%E1%85%A9%E1%86%AB%E1%84%92%E1%85%A8%E1%84%8B%E1%85%AF%E1%86%AB_Section4(%E1%84%89%E1%85%AE%E1%84%8C%E1%85%A5%E1%86%BC).pdf)
- [ํ๋ก์ ํธ ๋ฐํ ์์ ๋งํฌ](https://youtu.be/kNREu3zikb4)

## 5. Reference
* https://github.com/bckenstler/TheresWaldo
* https://www.flickr.com/photos/153621475@N06/albums/72157684946674930/with/36420949126/
* https://www.kaggle.com/kairess/find-waldo
