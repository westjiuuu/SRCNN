# SRCNN (Super-Resolution Convolutional Neural Network)

Paper: Dong et al., *Image Super-Resolution Using Deep Convolutional Networks*, ECCV 2014  

SRCNN을 PyTorch로 재구현하고, T91 / Set5 데이터셋을 활용하여 **x2, x3, x4 업샘플링 성능 평가**를 수행한 코드입니다.  

## Experimental Results

### x2 (400 Epochs, Adam, Loss: 0.000633)
| Metric | Bicubic | SRCNN | Paper |
|--------|---------|-------|-------|
| **PSNR (dB)** | 33.68 | **35.99** | 36.66 |
| **SSIM**      | 0.9368 | **0.9548** | 0.9542 |

---

### x3 (400 Epochs, Adam, Loss: 0.001316)
| Metric | Bicubic | SRCNN | Paper |
|--------|---------|-------|-------|
| **PSNR (dB)** | 29.81 | **32.16** | 32.75 |
| **SSIM**      | 0.8711 | **0.9102** | 0.9090 |

---

### x4 (1000 Epochs, Adam, Loss: 0.001906)
| Metric | Bicubic | SRCNN | Paper |
|--------|---------|-------|-------|
| **PSNR (dB)** | 27.92 | **29.72** | 30.49 |
| **SSIM**      | 0.8076 | **0.8489** | 0.8628 |
