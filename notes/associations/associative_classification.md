## CPAR: Classification based on Predictive Association Rules

[Yin, X., & Han, J. (2003, May). CPAR: Classification based on predictive association rules. In Proceedings of the 2003 SIAM International Conference on Data Mining (pp. 331-335). Society for Industrial and Applied Mathematics.][CPAR_2003]

Rule based classification의 대략적인 소개가 나옴. 

First Order Inductive Learner (FOIL)의 경우는 rule expansion을 위한 gain을 계산하는데 매우 비싸기 때문에 Predictive Rule Mining (PRM)에서 PNArray라는 구조를 제안하였음. 

PRM의 경우 Decision Tree와 같이 greedy하게 하나의 변수를 기준으로 rules을 expansion 시키는데, greedy하게 best인 rules가 전체의 best rules은 아니기 때문에 overfitting 이 발생하고, 이로 인하여 performance가 떨어진다고 주장. 

Rules이 표현하는 범위에 overlap을 두고 weight decaying을 함으로써, 좀 더 global best rules이 될 수 있도록 유도. 

그러나 UCI dataset으로 평가한 성능에서 성능이 크게 오르지 않음, 심지아 RIPPER라는 방법은 규칙의 개수가 매우 적음에도 불구하고 비슷한 성능을 보이고 있음. 

<p align="center"><img src="./figs/cpar_vs_ripper0.png" width="300"></p>
<p align="center"><img src="./figs/cpar_vs_ripper1.png" width="300"></p>

이 논문은 매우 중요한 논문은 아니라고 판단, RIPPER나 survey paper를 찾아보기로 함. 


## Fast effective rule induction

[Cohen, W. W. (1995, July). Fast effective rule induction. In Proceedings of the twelfth international conference on machine learning (pp. 115-123).][RIPPER_1995]

[CPAR_2003]: https://www.researchgate.net/profile/Xiaoxin_Yin/publication/2560610_CPAR_Classification_based_on_Predictive_Association_Rules/links/54341fe70cf2bf1f1f27b8a6.pdf

[RIPPER_1995]: https://pdfs.semanticscholar.org/2d5f/21740caf3c834101060b7a6d505780a299dd.pdf