# VideoBased-SurgicalSkillAssessment

Please follow these steps on the Google Colab:
1) Run three "Video2ResNet_(KT, NP, SU).ipynb" files to create pickle files as the input of the deep network. Each video frame after passing through the ResNet50 pretrained model over the ImageNet produces 2048 features(note: the classification head is removed). All of the 2048 time-series of features with the length of the input video will be passed through FFT block. The absolute value of the first 300 FFT coefficients for all of 2048 features will be saved as pickle files as the input of the deep network. Save all generated files (~600 Mb) in a folder on your Google Drive.
Note: Do not run the whole file to avoid disk error.
2) In "JIGSAWS_videoClassification.ipynb" set the path of the Google Drive folder containing generated files from step 1 in the string variable "path" and run the other sections of the code with your preferable adjustments.
