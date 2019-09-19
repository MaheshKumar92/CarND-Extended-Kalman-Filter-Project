# Extended Kalman Filter Project Starter Code
Self-Driving Car Engineer Nanodegree Program

## Steps
1. read measurement data.
2. Initialize X, P, F and Q Matrixes. (For lidar initilize X directly, For radar calculate cartesian values from polar values)
3. call `predict()` function. and update X and P. (Same for lidar and radar)
4. call `update()` function for lidar and call `updateEKF()` for radar. Both functions are almost same except later uses jacobian H. because radar has
   nolinear measrement function.
5. calculate RMSE (root mean square error)


## Basic Build Instructions
1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make` 
   * On windows, you may need to run: `cmake .. -G "Unix Makefiles" && make`
4. Run it: `./ExtendedKF ` 
5. Already these steps are done, and you can directly run ExtendedKF. 
