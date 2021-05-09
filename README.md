# CellPin


## 배경
---
- 작년부터 지금까지도 문제가 되고 있는 COVID 19 사태의 원인은 신종바이러스 SARS-CoV2이다. 신종바이러스에 대한 발빠른 검출과 연구가 매우 중요해지고 있다. 바이러스의 연구를 위해서는 바이러스의 정량구하는 것은 중요한 부분이다. 하지만, 바이러스는 눈에 보이지 않을 뿐더러 광학현미경으로도 거의 대부분이 확인이 불가능하다. 따라서, 바이러스의 농도를 달리하여 세포에 감염시킨 후 CPE(Cytopathic Effect)의 여부를 통해 바이러스의 역가를 구하는 TCID 50(Tissue Culture Infective Dose 50) 방법을 일반적으로 사용한다. CPE는 연구가 미숙한 연구자가 확인할 때나 숙련된 연구자라도 다루지 않은 바이러스의 CPE를 확인할 때 어려움이 있을 수 있다. 또한, 정확하게 TCID를 구하는 방법도 복잡한 계산과정이 요구된다. 따라서, CPE의 여부를 판단해주는 객관적인 지표와 정확하게 TCID를 구하는 계산해주는 웹사이트가 있다면 바이러스 연구에 도움이 될 것이다.

## 기능
---
- 바이러스의 CPE(Cytopathic Effect)를 통해서 정상세포와 바이러스에 감염된 세포의 image를 classification 해주는 image classifier
- image를 업로드 할 시 바이러스 감염여부를 판단
- 바이러스 정량방법 중 하나인 TCID 50(Tissue Culture Infective Dose 50)를 구해주는 Calculator

## 참여인원 및 담당역할
---
- [이혜성](https://github.com/gotjd709)
- [김정우](https://github.com/mochafreddo)
- [이동훈](https://github.com/Soah-1994)
- [유기표](https://github.com/fbrlvy87)


## 배경지식
---

#### CPE(Cytopathic Effect)란?

![image](https://user-images.githubusercontent.com/70703320/117326870-0926d280-aecd-11eb-97c4-b96ca4d34569.png)
[출처](https://cytosmart.com/resources/virus-induced-cytopathic-effect)

- 세포가 바이러스에 감염되었을 때 나타나는 특징적인 병증

#### TCID 50(Tissue Culture Infective Dose 50)을 구하는 방법

- TCID 50 이란 대개는 10배수로 희석시킨 바이러스 부유액을 각 배수별로 5개 이상(대개 8-10 test units)의 세포단층, egg, 동물 등에 접종시켜 50%를 감염시키는 바이러스 희석배수를 titer로 나타낸 것

![스크린샷, 2021-05-09 22-40-30](https://user-images.githubusercontent.com/70703320/117574347-a70ddd80-b117-11eb-862e-340c3859096a.png)

#### 시도할 모델

- [VGG19 Net](https://arxiv.org/pdf/1409.1556.pdf)
- [ResNet 50](https://arxiv.org/pdf/1512.03385.pdf)
- [U Net ++](https://arxiv.org/pdf/1807.10165.pdf)
- [Mobile-Unet](https://journals.sagepub.com/doi/pdf/10.1177/0040517520928604?casa_token=9gXXnyqqT-8AAAAA:EnmwdVP-MHUpb22ke29eSi7fcW3Vq37BRnI361rr3EflVKS8VBSMoeHHJ_4TgVwkK42HyAH4f_DM3W8)




## Reference
---
- Wang, Ting-En et al. "Differentiation of Cytopathic Effects (CPE) induced by influenza virus infection using deep Convolutional Neural Networks (CNN)." PLoS computational biology vol. 16,5 e1007883. 13 May. 2020, doi:10.1371/journal.pcbi.1007883
- 강정욱. "바이러스의 정량법" Korean J Clin Microbiol 2001 ; 4 : 1-4
