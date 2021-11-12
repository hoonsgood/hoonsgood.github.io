---
title: "QC NR NonSignaling"
excerpt: ""

categories:
  - RF
tags:
  - QC
  - NR
  - NonSignaling
last_modified_at: 2021-11-08 16:00:00 +0900
toc: true
toc_label: "Contents"
toc_icon: "cog"
toc_sticky: true
---

## NonSignalig vs RF NonSignaling

- Frequency Sync를 맞추기 위해 장비에서 Frame단위의 waveform을 단말에 Tx하고 단말에서는 이를 받아서 Frequency Sync를 맞춘다.
- 기존 NonSignaling : Frequency Sync를 맞추고, 단말을 시리얼 또는 TCP/IP와 같은 인터페이스를 통해 컨트롤하여 테스트하는 방법
- RF NonSignaling : Frequency Sync를 맞추지 않고, 단말을 시리얼 또는 TCP/IP와 같은 인터페이스를 통해 직접 컨트롤하여 테스트하는 방법
- QC NR부터는 RF NonSignaling만 지원을 한다.

## Rx 테스트 방법

- Sync를 맞추는 작업이 없기 때문에 Rx 에러율 측정을 할 수 없다.
- SNR(Signal to Noise Ratio)와 FER(Frame Error Ratio)의 상관관계를 통해 Estimated Sensitivity를 측정하여 Rx측정

### SNR과 FER의 상관관계

- SNR의 값이 높아질수록 FER은 낮아지고, SNR의 값이 낮아질수록 FER은 높아진다.
- 이 알고리즘을 이용하여 Estimated Sensitivity를 측정한다.

## Tx 테스트 방법

- Tx 보정
- Rx 보정
- Don't care : Frequency Error limit line을 2~3ppm으로 잡아서 테스트
