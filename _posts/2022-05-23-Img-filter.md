---
layout: post
title: "[Pyhthon] Pillow로 이미지 필터 씌우기"
---

## Pillow 라이브러리 불러오기

> 
> from PIL import Image, ImageFilter, ImageEnhance, ImageOps

## 이미지 파일 열기, 회전, 흑백 변환, 손그림 필터
> img = Image.open("/Users/image/photo/output01.jpg")
>
> img.show()
> 
> img = img.rotate(45, expand = True)
>
> img.show()
> 
> img = ImageEnhance.Brightness(img).enhance(0.4)
>
> img.show()
> 
> 
> img = ImageOps.grayscale(img)
>
> img.show()
> 
> img = img.filter(Image.Filter.EMBOSS)
>
> img.show()
> 
> 
> img = Image.open("/Users/image/photo/picture73.jpg")
> 
> img = img.filter(ImageFilter.CONTOUR)
>
> img.show()
> 