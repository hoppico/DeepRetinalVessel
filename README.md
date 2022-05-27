# DeepRetinalVessel
## Using Cauchy Matched Filter to Improve the Detection of Retinal Vessel Via Convolutional Neural Networks

In 2011, I finished my master's investigations on proposing a new kernel for matched filter to detect retinal vessels. The details of this study was published [HERE](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3967450/).
Years later in 2021, I decided to revisit my work, but this time I intended to equipped the detection with Convolutional Neural Networks. 

## Idea

The idea is easy and straight-forward. Since both the vessels and the retinal background are red, using original images may not improve the detection accuracy. Therefore, I decided to perform a preprocessing on the images considering my original work.

![Pipeline of preprocessing](https://github.com/hoppico/DeepRetinalVessel/blob/master/Images/pipeline.png?raw=true)

Simply said, I removed the red and blue channels of the images, and replace them with two preprocessed images. For more details, the red and blue channel are replaced with Cauchy and Gaussian matched filters, aiming to provide more features for the CNN to distinguish between the vessels and retinal background.

![Results](https://github.com/hoppico/DeepRetinalVessel/blob/master/Images/TheWorkEntirely.PNG?raw=true)
![enter image description here](https://github.com/hoppico/DeepRetinalVessel/blob/master/Images/Results.png?raw=true)
# Implementations

The CNN implementation is not mine, and I used an open source code available [Here](https://github.com/DeepTrial/Retina-VesselNet). 

For those who are interested to know more, I have to say that I was a part of research carried out by a group of researchers in the University of Jazan. But since we had an agreement, I did not participated in their publication, but the copyright of the code is mine. You are allowed to have the code, change and distribute it.

The work is published [here](https://www.frontiersin.org/articles/10.3389/fpubh.2022.858327/full).

IMPORTANT DISCLAIMER: Please pay attention that this is a research work, and it SHOULD NOT be applied in real medical diagnosis, or any real medical purposes. 

# Copyright

MIT License. Work, enjoy, and share
