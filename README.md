# 1. Getting NGC

download ngc
<br/>

```wget --content-disposition https://api.ngc.nvidia.com/v2/resources/nvidia/ngc-apps/ngc_cli/versions/3.41.4/files/ngccli_linux.zip -O ngccli_linux.zip && unzip ngccli_linux.zip```

give permission
<br/>

```chmod u+x ngc-cli/ngc```

run
<br/>

```ngc config set```
<br/>
then enter your credential

## resources
tutorial video: https://resources.nvidia.com/en-us-riva-tutorials-briefcase/riva-quick-start-guide
geting NVIDIA api key:https://org.ngc.nvidia.com/setup/api-key

# 2. Getting and Starting RIVA container

```ngc registry resource download-version nvidia/riva/riva_quickstart:2.15.0```<br/>
```cd riva_quickstart_v2.15.0```<br/>
```bash riva_init.sh```<br/>
```bash riva_start.sh```<br/>

after you have done using the container, don't forget to run<br/>
```bash riva_stop.sh```

notes that in the code we used port 8889, you might have to edit that in either riva_quickstart_v2.15.0/config.sh or the code.
We already provided the config.sh file in this repository so you can just copy and paste the file.

# 3. getting FoodRAG

basically clone the repository.<br/>
```git clone https://github.com/NVAITC-APS/FoodRAG/tree/dev_POC```<br/>

getting requirements<br/>
```fresh_install_requirements.txt```<br/>

start the application<br/>
```streamlit run main.py```<br/>

# 4. Extra Scripts

we also archived the code used for training, finetuning, inferecing and the speech emotion recognition models for this project [here](https://github.com/catsudon/tensorflow-LSTM-SER) 