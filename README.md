# RGBD-DSO Direct Sparse Odometry with RGB-D Cameras for Indoor Scenes

### 1. Related Papers
* **RGB-D DSO: Direct Sparse Odometry with RGB-D Cameras for Indoor Scenes**, *Yuan Z, Cheng K, Tang J, Yang X*, In IEEE Transactions on Multimedia, 2021

### 2. Installation

	git clone https://github.com/HustCK/RGBD-DSO.git

#### 2.1 Required Dependencies

##### 2.1.1 Suitesparse 
Install with

		sudo apt-get install libsuitesparse-dev libboost-all-dev

##### 2.1.2 Eigen3
Eigen 3.2.8, Follow [Eigen Installation](http://eigen.tuxfamily.org/index.php?title=Main_Page).

##### 2.1.3 OpenCV
OpenCV 2.4.9, Follow [OpenCV Installation](https://opencv.org/releases/page/7/).

##### 2.1.4 Pangolin
Pangolin, Follow [Pangolin Installation](https://github.com/stevenlovegrove/Pangolin).

##### 2.1.5 ziplib
Install with

		sudo apt-get install zlib1g-dev
		cd dso/thirdparty
		tar -zxvf libzip-1.1.1.tar.gz
		cd libzip-1.1.1/
		./configure
		make
		sudo make install
		sudo cp lib/zipconf.h /usr/local/include/zipconf.h
	
#### 2.2 Build

		cd RGBD-DSO
		mkdir build
		cd build
		cmake ..
		make -j4
		
### 3. Usage

#### 3.1 Dataset Format
Let's take TUM RGB-D as an example.
