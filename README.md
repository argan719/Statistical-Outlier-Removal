# Automated 2D Blueprint Generation from 3D Point Clouds

#### This project showcases an end-to-end pipeline that transforms raw, noisy 3D point cloud data into clean, structured 2D architectural floor plans.
<br>

Original author: Hyungtae Lim (shapelim@kaist.ac.kr) https://github.com/LimHyungTae/pcl_tutorial
<br><br>




### Description
- <b>Denoising:</b> Applies a Statistical Outlier Removal(SOR) filter to clean the input 3D data.
- <b>2D Projection:</b> Converts the filtered 3D point cloud into a 2D top-down image by removing the Z-axis.
- <b>Build Improvement:</b> The project was refactored with a standalone CMkae build for the SOR module to improve modularity and simplify compilation.

<br>


### Input: pcd / Output: result.png

<br>

### Compile

~/sor/build$ cmake .. <br>
~/sor/build$ make <br>

### Run

~/sor/build$ ./lec07_sor <br><br>



### Result <br>
(Before/ After) <br>
<img width="613" alt="image" src="https://github.com/argan719/SOR/assets/64789601/1c30fa74-ef9f-452f-a082-de2318f6d840">
<img width="613" alt="image" src="https://github.com/argan719/SOR/assets/64789601/3372c4f8-9c57-4111-ad80-f33225581e4c">
<img width="612" alt="image" src="https://github.com/argan719/SOR/assets/64789601/7256ebf6-ff7b-4de3-a2c6-13cee7ff2015">
<img width="612" alt="image" src="https://github.com/argan719/SOR/assets/64789601/15a1b076-d305-4d92-8265-1461ca7e0856">

