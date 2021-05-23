# VideoBased-SurgicalSkillAssessment

Please follow these steps on the Google Colab:
1) Run three Video2ResNet_(KT,NP,SU) files to create pickle files as the input of the deep network. Each video frame after passing through the ResNet50 pretrained model over ImageNet, produces 2048 features(note: the classification head is removed). All of the 2048 time-series of features with the length of the input video will be passed though FFT block. The absolute value of first 300 FFT coefficients for all of 2048 features will be saved as pickle files as the input of the deep network.
### Note: 
3) de

