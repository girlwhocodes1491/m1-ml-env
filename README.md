# m1-ml-env
Setup ML Env for M1 Mac
In this repo you will find some step-by-step simple guide to setup a Machine Learning Environment in M1 Macbook Air.

## Setup tensorflow Environment

1. Donwload [Miniforge3](https://github.com/conda-forge/miniforge)
2. Install Miniforge3 in the home directory
  ```
  chmod +x ~/Downloads/Miniforge3-MacOSX-arm64.sh
  sh ~/Downloads/Miniforge3-MacOSX-arm64.sh
  source ~/miniforge3/bin/activate
  ```
3. Create TensorFlow dir
  ```
  mkdir tensorflow-testing
  cd tensorflow-testing
  ```
4. Create Conda Env
  ```
  conda create --prefix ./env python=3.8
  ```
5. Activate Conda Env
  ```
  conda activate ./env
  ```
 6. Get TensorFlow Dependencies
  ```
  conda install -c apple tensorflow-deps
  ```
 7. Install Base TensorFlow
  ```
  python -m pip install tensorflow-macos
  ```
 8. Install Apple Metal for GPU acceleration 
  ```
  python -m pip install tensorflow-metal
  ```
 9. Install most used Data Science Libraries
  ```
  conda install jupyter pandas numpy matplotlib scikit-learn
  ```
 10. Start Jupyter
  ```
  jupyter notebook
   ```
 



