# Colorizing_black&White_images
neural network to color black and white photos

## Result

<p ><img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/400%20images%201000%20epochs/1.png" width="255px">
    <img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/400%20images%201000%20epochs/50.png"400px">
    <img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/untitled%20folder/11.png"400px">
    <img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/untitled%20folder/20.png"400px">
    <img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/untitled%20folder/68.png">
    <img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/untitled%20folder/15.png">


**My test dataset was big enough to find few good results** 

**Note:**  A large majority of the images are lightly colored in brown. As color brown gives a much lower loss value.  A limited and basic dataset makes better outcomes.



## Model-1 
 An image translated into LAB pixel values. It also builds a core intuition for how the network learns. How the network compares the input with the output and adjusts the network. 

<p ><img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/10%20epochs/dataset0.png" width="255px">
    <img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/10%20epochs/dataset4(2).png"400px">



</p>

In this version,result images are colored brown as the network is not big enough and not been trained for longer duration. This neural network builds an intuition for the purpose of the final version and is simple enough to implement easily. 

## Model-2 
The full version adds information from a pre-trained classifier. It then learns to combine that information with the black and white photo. It gives the network more confidence to color the image. Otherwise, it tends to default to the safest color, brown.



<p><img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/600%20epochs/0.png" width="350px">
    <img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/400%20images%201000%20epochs/45.png" width="350px">
    <img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/400%20images%201000%20epochs/52.png" width="350px">
    <img src="https://github.com/tejasbana/Colorizing_black-White_images/blob/master/experiments/400%20images%201000%20epochs/85.png" width="350px">

</p>

You'll start getting some results after about 8 hours on a google-colab free GPU but its hard to train it for longer period of time with large dataset as google-colab gives only 12gb ram, which often overloads and crashes with this network.

## Acknowledgments
- Thanks to [emilwallner's](https://github.com/emilwallner/Coloring-greyscale-images) article and work in this project , kindly follow his article to understand in depth.
- [Dataset](https://www.floydhub.com/emilwallner/datasets/colornet/2/images)


**Currently Learning GANS to build a better model.**
