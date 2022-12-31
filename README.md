# WwiseFilePackager
一个用于读取wwise的PCK文件的python脚本

不自带bnk解析

原本是准备筛选原神音乐而写的文件

# GUIDE
Check out this mini guide on how to repack .pck files for genshin impact
1. First, follow the guide in the picture IMG1 (I'm not exactly sure whose guide this is  I took it from AGRG by user @undefined) (Link to the unpacker: https://github.com/mortalis13/Wwise-Unpacker/blob/master/Tools/wwise_pck_extractor.bms) or use Voice_Files_EN.json (According to my feelings, from the data for the Grasscooter 3.3, I collected links to sound files from 2.8 ~ 3.0)
![alt text](https://raw.githubusercontent.com/DiXiaoO/WwiseFilePackager/main/GUIDE_File/IMG1.png)
2. Unpack the .pck file using the 1 step tool

3. Creating new voiceover files in .wav format

4. So! Now we know which file contains what. Now we need to convert the created .wav file to .wem, which we will use to repack the voice acting.
4.1 Download Wwise from the official website https://www.audiokinetic.com/en/products/wwise/
4.2  Download the latest version of Wwise IMG2
![alt text](https://raw.githubusercontent.com/DiXiaoO/WwiseFilePackager/main/GUIDE_File/IMG2.png)
4.3 We create a new project IMG3
![alt text](https://raw.githubusercontent.com/DiXiaoO/WwiseFilePackager/main/GUIDE_File/IMG3.png)
4.4 IMG4
![alt text](https://raw.githubusercontent.com/DiXiaoO/WwiseFilePackager/main/GUIDE_File/IMG4.png)
4.5 Importing audio files IMG5
![alt text](https://raw.githubusercontent.com/DiXiaoO/WwiseFilePackager/main/GUIDE_File/IMG5.png)
4.6 We take steps as in the picture IMG6 (I'm too lazy to describe in detail. I hope everything is clear here)
4.7 Now RMB on file 1 on IMG6 >>> Convert...
![alt text](https://raw.githubusercontent.com/DiXiaoO/WwiseFilePackager/main/GUIDE_File/IMG6.png)
4.8 Go to the project folder and in the folder "Project name/.cache/Windows/SFX" there will be .wem files

5. Now the fun part!!! Replacing sound in .pck files
5.1 Files such as MusicN.pck and StreamedN.pck can be repacked using wwiseutil (It seems like everything is clear and not complicated there)
5.2 Download https://github.com/BUnipendix/WwiseFilePackager/blob/main/FilePackager.py  (Thanks @unipendix)
5.3 Download and unpack PCKrepack.zip and move the downloaded file there
5.4 In the input_pck folder put the .pck file you want to modify
      In the wem folder create a folder named .pck file (without .pck extension) (example 1001.pck >> 1001)
5.5 Download Python and run repack.py (If there are errors, just install the dependencies)
5.6 new .pck should have appeared in output_pck
Write if something is not clear (I wrote this guide with the help of a translator at 3 am 💀)
