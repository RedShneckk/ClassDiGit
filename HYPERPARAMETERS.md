#  MLP Model Results

|Trial|BATCH|  LR   |STEPS|LR_DECAY| PAT|ANGLE| SCALE| SHIFT|SAMPL|   Acc   |  Notes 
|  1  | 256 | 0.010 | 150 |  0.90  | 50 |  10 | 0.05 | 0.05 |  1  | 96.55 % | Baseline training
|  2  | 256 | 0.010 | 180 |  0.90  | 50 |  10 | 0.05 | 0.05 |  1  | 96.56 % |+30 training steps 
|  3  | 256 | 0.015 | 150 |  0.90  | 50 |  10 | 0.05 | 0.05 |  1  | 96.78 % | Increased learning rate
|  4  | 256 | 0.015 | 180 |  0.90  | 50 |  10 | 0.05 | 0.05 |  1  | 96.37 % | +30 steps, LR tuned to 0.015 
|  5  | 256 | 0.0125| 150 |  0.90  | 50 |  10 | 0.05 | 0.05 |  1  | 96.64 % | Lower learning rate (stability)
|  6  | 256 | 0.015 | 150 |  0.90  | 50 |  5  | 0.03 | 0.03 |  1  | 96.77 % | Reduced data augmentation 
|  7  | 256 | 0.015 | 150 |  0.90  | 50 |  5  | 0.03 | 0.03 |  0  | 96.63 % | Bilinear sampling test 
|  8  | 256 | 0.017 | 150 |  0.90  | 50 |  5  | 0.03 | 0.03 |  1  | 96.71 % | slightly higher LR

**Best MLP accuracy:** 96.78% (Trial 3)


#  CNN Model Results

|Trial|BATCH|  LR   |STEPS|LR_DECAY| PAT|ANGLE| SCALE| SHIFT|SAMPL|   Acc   | Notes 
|  1  | 512 | 0.020 | 120 |  0.90  | 50 |  10 | 0.05 | 0.05 |  1  | 98.93 % |  Baseline CNN 
|  2  | 512 | 0.020 | 150 |  0.90  | 50 |  10 | 0.05 | 0.05 |  1  | 98.89 % |  +30 training steps 
|  3  | 512 | 0.010 | 150 |  0.90  | 50 |  10 | 0.05 | 0.05 |  1  | 98.83 % | Lower learning rate/lower convergence
|  4  | 256 | 0.020 | 150 |  0.90  | 50 |  10 | 0.05 | 0.05 |  1  | 98.36 % | Smaller batch size 
|  5  | 512 | 0.015 | 150 |  0.85  | 50 |  10 | 0.05 | 0.05 |  1  | 98.70 % | Stronger learning rate decay
|  6  | 512 | 0.015 | 150 |  0.85  | 50 |  5  | 0.03 | 0.03 |  1  | 98.76 % | Reduced augmentation
|  7  | 512 | 0.015 | 150 |  0.85  | 50 |  5  | 0.03 | 0.03 |  0  | 98.81 % | Bilinear sampling variant 
|  8  | 512 | 0.015 | 180 |  0.85  | 50 |  10 | 0.05 | 0.05 |  1  | 98.97 % | Steps 180 
|  9  | 512 | 0.020 | 180 |  0.90  | 50 |  10 | 0.05 | 0.05 |  1  | 99.09 % | Baseline + Steps 180 

**Best CNN accuracy:** 99.09% (Trial 9)


📄 Back to [`README.md`](./README.md)