# convergent-learning
This is my own implementation of a part of this paper http://arxiv.org/pdf/1511.07543v3.pdf 
I am not one of the authors and have no relation or copyrights regarding the original work. This is simply my own implementation of 
a part of the paper I did for a project, and found it useful hence I am sharing.


This is the implementation of the semi matching of activations from two VGG 16s. The net can be substituted by any other network. I
have followed the same approach as described in the paper of taking max correlations and then the mean.

This can be used to compare features learnt between two networks. This will allow you to analyse for yourself in which layer 
feature representations differ the most on networks trained on say two different tasks.

For a thorough understanding of the procedure and its implications I recommend going through the paper. It is a brilliant paper. In 
the paper the comparison is done between two AlexNets initiallized from random weights. But the correlation can be done 
between networks trained on different tasks also.

Here is an example where I have correlated two vgg networks on the task of classification. This is not on imagenet but a different dataset.

https://cloud.githubusercontent.com/assets/8834964/17228675/fbd53210-54e1-11e6-8eda-6433042fb275.png



This is the correlation comparison between vgg_vgg random and vgg vs a vgg trained on a different task.
https://cloud.githubusercontent.com/assets/8834964/17229053/d3ed42e0-54e3-11e6-9034-5dc20aad7ce5.png


This would show where that particular task features would affect the features the most. Once the layers of least correaltion are known, further steps of visualization can be used

The paper was published at ICLR 2016 and the authors are Yixuan Li , Jason Yosinski , Jeff Clune, Hod Lipson, & John Hopcroft
. Again I have nothing to do with the original work. This is just my own implementation of a part of their work over which I hold
no rights. 




