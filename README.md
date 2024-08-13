# control_python
<b>Dr.Varodom Toochinda</b>
<br>Dept. of Mechanical Engineering, Kasetsart University

<img src="https://drive.google.com/uc?id=1wb4TYWleOeD6bRXm5VTWdRqbuRWfmiRv" width=550 alt="Figure 3"/>

## Project Description
<p />The contents in this repository are converted from my 
<a href="https://scilabdotninja.wordpress.com/" target=_blank>Scilab.ninja</a> website. 
They are mostly Jupyter notebooks with Python code, using Scipy and Python Control Systems 
libraries. The emphasis is on control system analysis and design, and robotics. The materials could serve as classroom teaching aids in engineering schools where the subjects are offered.

<a href="https://dewdotninja.github.io/julia/control/julia_control.html" target=_blank>Julia version</a> is also available.

## Installation

<b>Requirement : </b> Python 3 with Scipy & Python control systems

<p />The notebooks can be executed on Google colab or on your local computer. 

<p />Execute the commands below to install Python control systems library in Colab
<pre>
!pip install control
</pre>

<p />I use Anaconda to setup a Jupyter notebook environment. The process is quite detailed.
Please consult some online information. 
<p />Suppose the environment name is <em>controlenv</em>. Python Control System can be installed by 
issuing the following commands in terminal window.
<pre>
conda activate controlenv
pip install control
</pre>

## Contents

### Control Engineering Basics
* [Module 1: Transfer Functions and Frequency Responses](ceb_m1.ipynb)
* [Module 2: Feedback Properties](ceb_m2.ipynb)
* [Module 3: Classical Loopshaping Design](ceb_m3.ipynb)
* [Module 4: PID Control](ceb_m4.ipynb)
* [Module 5: State Feedback](ceb_m5.ipynb)
* [Module 6: Discrete-time Control Systems](ceb_m6.ipynb)
* [Module 7: Continuous to Discrete Conversion Methods](ceb_m7.ipynb)
* Supplementary 
  * [PID Autotuning](autotuning.ipynb)
  * [Discrete-time PID implementation](adv_pid_implement.ipynb)
  * [Discrete-time PID implementation (object-oriented approach)](adv_pid_class_implement.ipynb)
  * [Feedforward Control](feedforward.ipynb)
  * [Least Square System Identification](lsid.ipynb)
  * [Implementing a general discrete-time transfer function](discrete_implement.ipynb)
  * [Implementing a general discrete-time transfer function (OOP approach)](discrete_implement_oop.ipynb)

## Updates

#### May 2024:

**Some syntax changes in Python control library 0.10.0 that needs to be corrected by you.**
* specify methods named control.zeros() and control.poles(). Some code in the notebook used
control.zero(), for example. 
* control.bode_plot() returns a single data object instead of 3 in previous version. So change 
```python
_,_,_ = ctl.bode_plot(S)
``` 
to 
``` python
_ = ctl.bode_plot(S)
```


<p align="center">
<img src="https://drive.google.com/thumbnail?id=13bzT7Rmy3bzvE7TiS0yfQo94kpxMuipF" alt="dewninja"/>
 <br>2024
</p>
