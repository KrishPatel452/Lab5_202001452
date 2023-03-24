# Krish Patel(202001452)

## Used tool for static analysis of code: mypy(Python)
## Used Github Repository: https://github.com/CT83/Rumaro.git

## Files used in static testing:
###   1. apis/utils.py
###   2. apis/config.py
###   3. apis/run_analysis.py
###   4. apis/\_\_init\_\_.py

## (A) apis/utils.py
### Screenshot of Result: <br />
![image](https://user-images.githubusercontent.com/78999910/227498901-80e7be48-71ef-4863-8ae7-2329b89a63d1.png)<br/>
### Lines which produced error: <br/>
![image](https://user-images.githubusercontent.com/78999910/227499119-86b844d2-64f5-4acb-91b3-8b03b54d0e17.png)<br/>
Here, Error :cannot find implementation or library stub for module named “cv2”, “numpy”. Shows that module mypy doesn’t contain any kind of special functions or
implementations to check these module’s implementations.<br/>
This stubs/implementations can be installed from respective module’s github repositories > stub folders.

## (B) apis/config.py
### Screenshot of Result: <br />
![image](https://user-images.githubusercontent.com/78999910/227499809-de426f11-57cd-4b25-b046-1e074c9d0f03.png)<br/>
### Lines which produced error: <br/>
![image](https://user-images.githubusercontent.com/78999910/227499910-83a36222-3118-449c-b209-6a9d1d65e362.png)
<br/>
Here, This error was caused by extra indent given at line 5 which can be observed here.
<br/>

## (C) apis/run_analysis.py
### Screenshot of Result: <br />
![image](https://user-images.githubusercontent.com/78999910/227500168-6e719a00-c6e2-455b-bea8-93d4ada23518.png)<br/>
### Lines which produced error: <br/>
![image](https://user-images.githubusercontent.com/78999910/227500265-b812e64a-2345-454e-83d9-83e1f84800ba.png)
<br/>
Here, This error was caused by extra indent given at line 5 which can be observed here.
<br/>

## (D) apis/\_\_init\_\_.py
### Screenshot of Result: <br />
![image](https://user-images.githubusercontent.com/78999910/227500556-47d88876-6d67-44d5-99d4-bda43baff76d.png)<br/>
<br/>
Here, module mypy couldn’t find any kind of error or warning; hence it doesn't show any error or warning message.
<br/>
