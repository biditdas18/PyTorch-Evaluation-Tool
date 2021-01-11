# Instructions For Using The Tool
1. The main file of interest here is torch_eva.py where all the evaluation will be carried out
2. For ease of usage please put your dataset and the trained model inside the PyTorch-Evaluation-Tool folder
3. If the above step is not possible due to some reasons make sure to provide appropriate path to dataset and saved model at appropriate places when prompted by the comment section of the code 
4. There are 2 places in the code where user input is needed i.e. TEST_DATA_PATH and model. Those sections are clearly marked in the comment section of the code
5. While training your model make sure to save the model using torch.jit.save(), that way you won't need the model architecture while evaluating your code.
6. In case you have already saved your model using some other method, space has been provided to provide the user's model architecture
7. This tool doesn't generate any loss vs epoch graph or accuray vs epoch graph as those details are recorded while training the model and can't be retrieved from saved model.
8. If everything works fine you should get the following results:<br/>
    a) Test accuracy will be printed<br/>
    b) The confusion matrix will be printed<br/>
    c) A plot of the confusion matrix<br/>
    d) Another plot of the confusion matrix in a heatmap <br/>
    e) A Plot of the ROC curve <br/>
    f) Classification report will be printed<br/>
    g) An interactive table of classification report will be generated in Bokeh Table <br/>
    
9. Tensorboard can be also run if you already have the saved logs
10. To run the tensorboard use the following steps:<br/>
    a) Go to the folder containing the logs using command prompt<br/>
    b) Run the following command:<br/>
        tensorboard --logdir logs<br/>
    c) You will get a host similar to the one below:<br/>
        http://localhost:6006/ <br/>
    d) Paste it in your browser and run to view the tensorboard.<br/>
    e) A sample logs file named as logs is provided in Project1_Final folder for users to run and see how Tensorboard works
   
11. This tool is for evaluation of simple pytorch models and may not be able to handle specialized evaluation methods for which custom changes are needed
12. As a simple use case project1_Final already has a dummy dataset, and a dummy saved model so that users can see how the model is working before evaluation on their own dataset and saved model

   
