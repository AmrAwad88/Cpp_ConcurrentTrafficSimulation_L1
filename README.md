# Cpp_ConcurrentTrafficSimulation_L1
This is a training for writing a concurrent program in C++

This is the first lesson's excercise. The code explanation is provided by Prof. Andreas Haja in the Youtube links below:
https://www.youtube.com/watch?v=iifZEu0ctxc&t=1s&ab_channel=Udacity  \
https://www.youtube.com/watch?v=OwiKpGYN9wI&ab_channel=Udacity

## The Project's Description:

### Project Tasks
**Task L1.1 :** In the base class TrafficObject, set up a thread barrier in its destructor that ensures that all the thread objects in the member vector _threads are joined. \
*Developer Comment: the _id counter is a unique object's counter and it could be used to identify the thread from the _threads array to be set as a barrier.*

**Task L1.2 :** In the Vehicle class, start a thread with the member function drive and the object this as the launch parameters. Also, add the created thread into the _thread vector of the parent class.\
*Developer Comment: the tasks id are detributed in a sequential manner, which means that all the vehicle's indecies are occyping a certain range and emplace_back could be used to buffer all the threads in the _threads array.*

**Task L1.3 :** Vary the number of simulated vehicles in main and use the top function on the terminal or the task manager of your system to observe the number of threads used by the simulation. \
*Developer Comment: the maximum number of vehicles is controlled before creating the vehicles instances.* 

You can find these tasks in the project_tasks.txt within the workspace as well.

### Build Instructions
To compile and run the code, create a build directory and use cmake and make as follows:
../L1_Project# mkdir build \
../L1_Project# cd build \
../L1_Project/build# cmake .. \
../L1_Project/build# make \
../L1_Project/build# ./traffic_simulation
