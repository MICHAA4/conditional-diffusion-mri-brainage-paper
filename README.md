<h1 align='center'>조건부 Diffusion 모델 기반 뇌 MRI 생성:
  
  뇌 연령 예측 정확도에 미치는 영향 분석 🧠</h1>

## 개요

딥러닝 기반 의료 영상 분석 기술의 발전은 뇌질환 진단 분야에 중요한 변화를 가져오고 있다. 하지만 의료 영상 데이터는 개인정보 보호 이슈와 데이터 부족 문제로 인해 모델 학습에 제약이 있으며, 이를 해결하기 위한 방안으로 생성형 AI, 특히 Diffusion 모델을 활용한 데이터 생성이 주목받고 있다. 본 연구에서는 성별, 나이, 뇌 슬라이스 번호를 조건으로 입력받는 조건부 2D 뇌 MRI 이미지를 생성하기 위해 Classifier-Free Guidance 기법을 적용하고, 전체 데이터의 20%를 비조건 상태로 구성하여 Diffusion 모델을 학습하였다. 생성된 합성 이미지의 시각적 품질(FID, SSIM)과 분석 성능(뇌 연령 예측 정확도) 간의 관계를 평가하기 위해, DeepBrainNet 모델을 fine-tuning하여 뇌 연령 예측 실험을 수행하였으며, Guidance Scale 변화에 따른 성능 차이를 분석하였다. 뇌 연령 예측은 노화 과정의 이상을 조기에 감지하고, 알츠하이머병과 같은 신경퇴행성 질환의 위험도를 평가하는 데 활용 가능한 주요 바이오마커로 주목받고 있다. 본 연구는 생성된 이미지가 이러한 예측 작업에 실제로 활용 가능한지를 정량적으로 검증함으로써, 생성형 AI 기반 MRI 영상이 의료 AI 모델의 학습 데이터 보강 수단으로서 지닌 잠재력을 평가하였다. 실험 결과, 시각적 품질이 높은 이미지가 반드시 높은 예측 성능으로 이어지지는 않음을 확인하였으며, 이는 합성 영상의 품질 평가에 있어 Downstream Task 기반의 실용적 지표가 반드시 고려되어야함을 시사한다.


## Development Period
2025.03 ~ 2025.04

## 👩🏻‍💻Member
<ul>
  <li><a href="https://github.com/MICHAA4">차성연</a> @Cha SeongYeon</li>
  <li>이호욱</a> @Lee Howook</li>
  <li>최용진</a> @Choi Yongjin</li>
</ul>

## Professor
<ul>
 <li><a href="https://wonhee-lee.github.io/">이원희</a> @Lee WonHee</li>
</ul>

## 📌Objectives
<ul>
 <li>Generate Realistic 2D Brain MRI Images Using Conditional Diffusion Model</li>
 <li>Apply Classifier-Free Guidance with Mixed Conditional/Unconditional Training</li>
 <li>Evaluate Synthetic Image Quality and Its Impact on Brain Age Prediction</li>
 <li>Explore Optimal Guidance Scale for Balancing Visual Fidelity and Predictive Utility</li>
</ul>

## Data
<ul>
  <li><a href="https://camcan-archive.mrc-cbu.cam.ac.uk/dataaccess/">Cam-CAN Dataset</a></li>
</ul>

## Result
(사진)

## How to Run
1. Clone MONAI repository
```
git clone https://github.com/Project-MONAI/MONAI
```
2. Clone DeepBrainNet repository
```
git clone https://github.com/vishnubashyam/DeepBrainNet
```
3. Clone this repository
```
git clone https://github.com/MICHAA4/conditional-diffusion-mri-brainage-paper
```
4. Go to src folder
5. Execute the files!

## Helpful Repositories
<ul>
  <li><a href="https://github.com/Project-MONAI/GenerativeModels">Project MONAI Generative Models</a> @Project-MONAI</li>
<li><a href="https://github.com/vishnubashyam/DeepBrainNet">DeepBrainNet</a> @DeepBrainNet</li>
</ul>
