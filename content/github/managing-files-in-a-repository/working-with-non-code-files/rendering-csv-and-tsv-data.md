=== Detailed Accuracy by Class ===

               TP Rate   FP Rate   Precision   Recall  F-Measure   ROC Area  Class
                 0.81      0.041      0.723     0.81      0.764      0.885    <20
                 0.817     0.029      0.895     0.817     0.855      0.894    <5
                 0.689     0.035      0.66      0.689     0.674      0.827    >20
                 0.954     0.064      0.951     0.954     0.952      0.945    None
Weighted Avg.    0.882     0.051      0.885     0.882     0.883      0.916

=== Confusion Matrix ===

   a   b   c   d   <-- classified as
  47   4   5   2 |   a = <20
   7  94   5   9 |   b = <5
   9   2  31   3 |   c = >20
   2   5   6 269 |   d = None

=== Generated Classifier Model ===

RandomTree
==========

BarPres < 1033.5
|   RelHumid < 75.5
|   |   WindDir = SW : <20 (2/0)
|   |   WindDir = SSW
|   |   |   MaxTemp < 18.25
|   |   |   |   RelHumid < 64 : None (8/0)
|   |   |   |   RelHumid >= 64
|   |   |   |   |   BarPres < 1025 : <5 (2/0)
|   |   |   |   |   BarPres >= 1025 : None (1/0)
|   |   |   MaxTemp >= 18.25
|   |   |   |   MaxTemp < 18.85
|   |   |   |   |   MinTemp < 8.05 : <20 (1/0)
|   |   |   |   |   MinTemp >= 8.05
|   |   |   |   |   |   RelHumid < 64 : <20 (1/0)
|   |   |   |   |   |   RelHumid >= 64 : <5 (1/0)
|   |   |   |   MaxTemp >= 18.85
|   |   |   |   |   BarPres < 1028
|   |   |   |   |   |   RelHumid < 61.5 : <20 (2/0)
|   |   |   |   |   |   RelHumid >= 61.5
|   |   |   |   |   |   |   MinTemp < 8.1 : <20 (4/0)
|   |   |   |   |   |   |   MinTemp >= 8.1 : None (4/0)
|   |   |   |   |   BarPres >= 1028 : None (4/0)
|   |   WindDir = SSE : None (8/0)
|   |   WindDir = ESE : <20 (0/0)
|   |   WindDir = E : <20 (0/0)
|   |   WindDir = NW
|   |   |   RelHumid < 74.5 : None (24/0)
|   |   |   RelHumid >= 74.5 : <5 (1/0)
|   |   WindDir = W
|   |   |   MaxTemp < 16.25
|   |   |   |   BarPres < 1026.5 : None (16/0)
|   |   |   |   BarPres >= 1026.5
|   |   |   |   |   MinTemp < 9.85 : None (1/0)
|   |   |   |   |   MinTemp >= 9.85 : <5 (3/0)
|   |   |   MaxTemp >= 16.25 : None (85/0)
|   |   WindDir = S : <5 (11/0)
|   |   WindDir = WNW : None (20/0)
|   |   WindDir = NNE : <20 (0/0)
|   |   WindDir = SE : <20 (0/0)
|   |   WindDir = WSW : None (11/0)
|   |   WindDir = NNW : None (12/0)
|   |   WindDir = NE : <20 (0/0)
|   RelHumid >= 75.5
|   |   MinTemp < 9.65
|   |   |   BarPres < 1016.5
|   |   |   |   WindDir = SW : <20 (11/0)
|   |   |   |   WindDir = SSW : <20 (0/0)
|   |   |   |   WindDir = SSE : <20 (0/0)
|   |   |   |   WindDir = ESE : <20 (0/0)
|   |   |   |   WindDir = E : <20 (0/0)
|   |   |   |   WindDir = NW : <20 (0/0)
|   |   |   |   WindDir = W : <20 (0/0)
|   |   |   |   WindDir = S : <20 (0/0)
|   |   |   |   WindDir = WNW : None (4/0)
|   |   |   |   WindDir = NNE : <20 (0/0)
|   |   |   |   WindDir = SE : <20 (0/0)
|   |   |   |   WindDir = WSW : <20 (0/0)
|   |   |   |   WindDir = NNW : <20 (0/0)
|   |   |   |   WindDir = NE : <20 (0/0)
|   |   |   BarPres >= 1016.5
|   |   |   |   RelHumid < 92.5
|   |   |   |   |   WindDir = SW
|   |   |   |   |   |   MinTemp < 9.55 : <20 (6/0)
|   |   |   |   |   |   MinTemp >= 9.55 : <5 (1/0)
|   |   |   |   |   WindDir = SSW
|   |   |   |   |   |   MinTemp < 9.3
|   |   |   |   |   |   |   MaxTemp < 18.05 : <5 (3/0)
|   |   |   |   |   |   |   MaxTemp >= 18.05 : <20 (2/0)
|   |   |   |   |   |   MinTemp >= 9.3 : None (1/0)
|   |   |   |   |   WindDir = SSE
|   |   |   |   |   |   MinTemp < 9.35 : >20 (3/0)
|   |   |   |   |   |   MinTemp >= 9.35 : <20 (1/0)
|   |   |   |   |   WindDir = ESE : <5 (1/0)
|   |   |   |   |   WindDir = E : <5 (1/0)
|   |   |   |   |   WindDir = NW : <5 (1/0)
|   |   |   |   |   WindDir = W
|   |   |   |   |   |   MinTemp < 5.85 : None (2/0)
|   |   |   |   |   |   MinTemp >= 5.85
|   |   |   |   |   |   |   BarPres < 1021.5 : None (2/0)
|   |   |   |   |   |   |   BarPres >= 1021.5 : <5 (5/0)
|   |   |   |   |   WindDir = S : <20 (0/0)
|   |   |   |   |   WindDir = WNW : <20 (0/0)
|   |   |   |   |   WindDir = NNE : <20 (0/0)
|   |   |   |   |   WindDir = SE : <20 (0/0)
|   |   |   |   |   WindDir = WSW : <20 (0/0)
|   |   |   |   |   WindDir = NNW : <20 (0/0)
|   |   |   |   |   WindDir = NE : None (1/0)
|   |   |   |   RelHumid >= 92.5
|   |   |   |   |   WindDir = SW : <20 (0/0)
|   |   |   |   |   WindDir = SSW : <20 (0/0)
|   |   |   |   |   WindDir = SSE : >20 (2/0)
|   |   |   |   |   WindDir = ESE : <5 (1/0)
|   |   |   |   |   WindDir = E : <20 (0/0)
|   |   |   |   |   WindDir = NW : <20 (0/0)
|   |   |   |   |   WindDir = W : <20 (0/0)
|   |   |   |   |   WindDir = S : <20 (0/0)
|   |   |   |   |   WindDir = WNW : <20 (0/0)
|   |   |   |   |   WindDir = NNE : <20 (0/0)
|   |   |   |   |   WindDir = SE : <20 (0/0)
|   |   |   |   |   WindDir = WSW : <20 (0/0)
|   |   |   |   |   WindDir = NNW : <20 (0/0)
|   |   |   |   |   WindDir = NE : None (4/0)
|   |   MinTemp >= 9.65
|   |   |   WindDir = SW
|   |   |   |   MinTemp < 10.8
|   |   |   |   |   MaxTemp < 13.85 : <5 (1/0)
|   |   |   |   |   MaxTemp >= 13.85
|   |   |   |   |   |   RelHumid < 80
|   |   |   |   |   |   |   RelHumid < 77.5 : <20 (1/0)
|   |   |   |   |   |   |   RelHumid >= 77.5 : <5 (1/0)
|   |   |   |   |   |   RelHumid >= 80 : <20 (2/0)
|   |   |   |   MinTemp >= 10.8 : <5 (8/0)
|   |   |   WindDir = SSW : <20 (0/0)
|   |   |   WindDir = SSE
|   |   |   |   RelHumid < 93.5 : >20 (2/0)
|   |   |   |   RelHumid >= 93.5 : <20 (7/0)
|   |   |   WindDir = ESE : <5 (3/0)
|   |   |   WindDir = E : <5 (3/0)
|   |   |   WindDir = NW : <5 (8/0)
|   |   |   WindDir = W
|   |   |   |   RelHumid < 90
|   |   |   |   |   MaxTemp < 16.6
|   |   |   |   |   |   MaxTemp < 15.55
|   |   |   |   |   |   |   MaxTemp < 13.55 : >20 (1/0)
|   |   |   |   |   |   |   MaxTemp >= 13.55
|   |   |   |   |   |   |   |   MinTemp < 12.5 : <5 (3/0)
|   |   |   |   |   |   |   |   MinTemp >= 12.5 : >20 (2/0)
|   |   |   |   |   |   MaxTemp >= 15.55
|   |   |   |   |   |   |   MinTemp < 10.95 : <5 (1/0)
|   |   |   |   |   |   |   MinTemp >= 10.95
|   |   |   |   |   |   |   |   MaxTemp < 16.05 : None (3/0)
|   |   |   |   |   |   |   |   MaxTemp >= 16.05 : >20 (2/0)
|   |   |   |   |   MaxTemp >= 16.6 : None (31/0)
|   |   |   |   RelHumid >= 90
|   |   |   |   |   MaxTemp < 16.85
|   |   |   |   |   |   MaxTemp < 15
|   |   |   |   |   |   |   MinTemp < 10.2 : >20 (1/0)
|   |   |   |   |   |   |   MinTemp >= 10.2
|   |   |   |   |   |   |   |   MinTemp < 10.65 : <5 (1/0)
|   |   |   |   |   |   |   |   MinTemp >= 10.65
|   |   |   |   |   |   |   |   |   MaxTemp < 14.1 : >20 (1/0)
|   |   |   |   |   |   |   |   |   MaxTemp >= 14.1 : <5 (1/0)
|   |   |   |   |   |   MaxTemp >= 15 : >20 (4/0)
|   |   |   |   |   MaxTemp >= 16.85 : None (4/0)
|   |   |   WindDir = S : <20 (0/0)
|   |   |   WindDir = WNW : <5 (3/0)
|   |   |   WindDir = NNE : <5 (5/0)
|   |   |   WindDir = SE : >20 (4/0)
|   |   |   WindDir = WSW : >20 (11/0)
|   |   |   WindDir = NNW : None (12/0)
|   |   |   WindDir = NE : None (5/0)
BarPres >= 1033.5
|   MinTemp < 12.95
|   |   WindDir = SW : <20 (2/0)
|   |   WindDir = SSW
|   |   |   RelHumid < 64.5 : None (4/0)
|   |   |   RelHumid >= 64.5
|   |   |   |   MaxTemp < 15.55 : None (1/0)
|   |   |   |   MaxTemp >= 15.55
|   |   |   |   |   MinTemp < 7.35 : <5 (3/0)
|   |   |   |   |   MinTemp >= 7.35
|   |   |   |   |   |   MinTemp < 7.95 : <20 (1/0)
|   |   |   |   |   |   MinTemp >= 7.95
|   |   |   |   |   |   |   BarPres < 1036.5 : <5 (2/0)
|   |   |   |   |   |   |   BarPres >= 1036.5 : <20 (1/0)
|   |   WindDir = SSE
|   |   |   MinTemp < 9.55
|   |   |   |   RelHumid < 76.5 : None (4/0)
|   |   |   |   RelHumid >= 76.5 : >20 (3/0)
|   |   |   MinTemp >= 9.55
|   |   |   |   MinTemp < 10.25
|   |   |   |   |   MaxTemp < 17.8 : <20 (1/0)
|   |   |   |   |   MaxTemp >= 17.8 : >20 (1/0)
|   |   |   |   MinTemp >= 10.25 : <20 (13/0)
|   |   WindDir = ESE : <5 (7/0)
|   |   WindDir = E : <5 (8/0)
|   |   WindDir = NW : <5 (2/0)
|   |   WindDir = W
|   |   |   BarPres < 1035.5 : None (3/0)
|   |   |   BarPres >= 1035.5
|   |   |   |   MinTemp < 9.65 : <5 (4/0)
|   |   |   |   MinTemp >= 9.65
|   |   |   |   |   MaxTemp < 17.1 : <5 (6/0)
|   |   |   |   |   MaxTemp >= 17.1 : None (6/0)
|   |   WindDir = S : <20 (0/0)
|   |   WindDir = WNW : <5 (8/0)
|   |   WindDir = NNE : <5 (6/0)
|   |   WindDir = SE : >20 (3/0)
|   |   WindDir = WSW : <20 (0/0)
|   |   WindDir = NNW : <20 (0/0)
|   |   WindDir = NE : None (1/0)
|   MinTemp >= 12.95 : >20 (5/0)

Size of the tree : 193
