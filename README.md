# Tonic_Detection
we have worked on detecting the tonic or the base note of a singer by analyzing the background tanpura sound.

##Code and Idea Explanation:

1)Written a python script to download the high quality audio from youtube video and saves in .wav format. A Text file containing the Youtube link must be created in the same folder of the code file

2)Next block of code contains a function defined to trim the audio for specified length. The code trims the .wav file in different folders for different time frames for all the downloaded .wav files. You need to create this folder prior to running the code.

3)Next piece of code reads all the trimmed files from each of the folders and gives us the PCD for all the .wav files in that folder along with tonic notes, the output specific to the folder is stored in the .csv file in that folder itself.

4)A piece of code displays all the output .csv files from all the folders to have comparison of results for different audio length

5)Create a folder “recordings” and save all the files inside the folder. A piece of code converts .mp3 file to .wav file for further analysis.

6)Next corresponding piece of code creates a separate folder for each of the recordings, trims the audio file with different audio length and saves in the respective folder.

7)Now the task is to find the PCD, and tonic of each of the audio files and save the results in the .csv file in that folder itself.

8)Again a piece of code will help you to display all the .csv files from all the audio folders to see all the outputs together.

9)We have used librosa.pyin function to get a fundamental frequency of audio file frame wise. ~43 frames/sec = 43 f_0/sec which further gives us a PCD of audio files. The mode of the notes gives us the singer's tonic.

10)Results for various audio lengths are discussed in the PPT by comparing with the ground truth and the algorithm's output.

11)These codes can be further optimized to make a python module for easy usage. More information on our project can be found in PPT and commented code
