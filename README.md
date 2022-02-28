# traffic_prediction
## Problem Formulation
Traffic forecast is a typical time-series prediction problem, i.e. predicting the most likely traffic measurements (e.g. speed or traffic flow) in the next *H* time steps given the previous *M* observations from traffic network *G* as, 
<p align="center"><a href="https://www.codecogs.com/eqnedit.php?latex=\hat{v}_{t&plus;1},&space;...,&space;\hat{v}_{t&plus;H}=\mathop{\arg\max}_{v_{t&plus;1},&space;...,&space;v_{t&plus;H}}&space;\log&space;P(v_{t&plus;1},&space;...,v_{t&plus;H}|v_{t-M&plus;1},&space;...,v_t;G)." target="_blank"><img src="https://latex.codecogs.com/gif.latex?\hat{v}_{t&plus;1},&space;...,&space;\hat{v}_{t&plus;H}=\mathop{\arg\max}_{v_{t&plus;1},&space;...,&space;v_{t&plus;H}}&space;\log&space;P(v_{t&plus;1},&space;...,v_{t&plus;H}|v_{t-M&plus;1},&space;...,v_t;G)." title="\hat{v}_{t+1}, ..., \hat{v}_{t+H}=\mathop{\arg\max}_{v_{t+1}, ..., v_{t+H}} \log P(v_{t+1}, ...,v_{t+H}|v_{t-M+1}, ...,v_t;G)." /></a></p>
  
<p align="center"><img width="30%" height="30%" src="figures/Graph_Structured_Traffic_Data.png"></p> 
  
**Fig.1 Graph-structured traffic data.**  
Each indicates a frame of current traffic status at time step *t*, which is recorded in a graph-structured data matrix.
