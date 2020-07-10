# PACKAGING-YOUR-APPLICATION-WITH-OPENVINO

## This Content was Created by Intel Edge AI for IoT Developers UDACITY Nanodegree.

How to use the Deployment Manager present in OpenVINO to create a runtime package from our application.

## Packaging your Application
In this exercise we will see how we can use the Deployment Manager present in OpenVINO create a runtime package from our application. These packages can be easily sent to other 
hardware devices to be deployed.

In the video, I will be creating a runtime package of the <code>vtune_project</code> To follow along, you can either use the same project (it is present as a folder in this workspace), or 
you can upload your own application and create a runtime package from it.

You can find detailed instructions about the Deployment Manager [here](https://docs.openvinotoolkit.org/latest/_docs_install_guides_deployment_manager_tool.html).

Don't forget to source the OpenVino environment in your equipment and to navigate to the proper directories in the terminal.

Be sure to complete the following steps in the terminal:


Start the Deployment Manager in interactive mode
Select the hardware where you want to deploy your model
Select the folder containing your application code, models, and data

![image1](https://raw.githubusercontent.com/ARBUCHELI/PACKAGING-YOUR-APPLICATION-WITH-OPENVINO/master/imagen1.jpg)

![image2](https://raw.githubusercontent.com/ARBUCHELI/PACKAGING-YOUR-APPLICATION-WITH-OPENVINO/master/imagen2.jpg)

![image3](https://raw.githubusercontent.com/ARBUCHELI/PACKAGING-YOUR-APPLICATION-WITH-OPENVINO/master/imagen3.jpg)

![image4](https://raw.githubusercontent.com/ARBUCHELI/PACKAGING-YOUR-APPLICATION-WITH-OPENVINO/master/imagen4.jpg)

# Quiz Yourself
Which of the following can be included in the package created by the deployment manager?

(For each of the options below, get some mental practice by thinking about whether it should be included or not included, and then click on the button to see if you are correct.)

## Application Code
<strong>Included!<strong> Your application code is what loads the model and runs inference and it needs to be a part of the runtime package.
  
## Models
<code>Included!</code> Any model used by the application can be added to the runtime package. It is good practice to add this since your deployment device might not have an internet connection to be able to download the model. Moreover, by packaging both your application code and model together, you can get an idea of the total memory your deployment device will need.

## OpenVINO Toolkit
<strong>Included!</strong> The runtime package will contain all the necessary parts of the OpenVINO toolkit that is needed to run your application code.

## VTune Amplifier
<strong>Not included.</strong> The VTune Amplifier is used only to check whether your application has any hotspots and can be use to optimize your application code. This is not included in the runtime package and should only be used before deploying to check the performance of your application.


## Adaptation as a Repository: Andrés R. Bucheli.
