# Deepfakes-Detection-Papers
The papers of Deepfakes Detection.

# Deepfake Detection
## 1. Challenge

- [Google] [FaceForensics++ Benchmark](http://kaldir.vc.in.tum.de/faceforensics_benchmark/index.php)
- [Facebook] [Deepfake Detection Challenge]( https://www.kaggle.com/c/deepfake-detection-challenge/overview )
- [SenseTime] [DeeperForensics Challenge 2020 @ ECCV SenseHuman Workshop](https://competitions.codalab.org/competitions/25228#learn_the_details)

## 2. Survey

- [arXiv 2019] [Deep Learning for Deepfakes Creation and Detection](https://arxiv.org/abs/1909.11573)
- [ACM SIGSAC 2019] [Poster: Towards Robust Open-World Detection of Deepfakes](https://dl.acm.org/citation.cfm?doid=3319535.3363269)
- [arXiv 2020] [DeepFakes and Beyond: A Survey of Face Manipulation and Fake Detection](https://arxiv.org/abs/2001.00179)
- [arXiv 2020] [DeepFake Detection: Current Challenges and Next Steps](https://arxiv.org/abs/2003.09234)
- [arXiv 2020] [The Creation and Detection of Deepfakes: A Survey](https://arxiv.org/abs/2004.11138)

## 3. Dataset

- [Google] [FaceForensics++](https://github.com/ondyari/FaceForensics/tree/master/dataset)

- [ICCV 2019] [FaceForensics++: Learning to Detect Manipulated Facial Images](https://arxiv.org/abs/1901.08971)
   - 1000 original videos downloaded from youtube, 4000 manipulated videos generated based on *Deep-Fakes, Face2Face, FaceSwap and NeuralTextures*
   
- [Google] [DeepFakeDetection](https://ai.googleblog.com/2019/09/contributing-data-to-deepfake-detection.html)
  - over 363 original sequences from 28 paid actors in 16 different scenes
  - over 3000 manipulated videos using *Deep-Fakes*

- [Albany] [Celeb-DF](http://www.cs.albany.edu/~lsw/celeb-deepfakeforensics.html)
  - [CVPR 2020] [Celeb-DF: A Large-scale Challenging Dataset for DeepFake Forensics](https://arxiv.org/abs/1909.12962)
   - real and *DeepFake* synthesized videos having similar visual quality on par with those circulated online
   - 408 original videos collected from YouTube with subjects of different ages, ethic groups and genders, and 795 DeepFake videos synthesized from these real videos
  
-  [Facebook] [Deepfake Detection Challenge (DFDC) Dataset](https://www.kaggle.com/c/deepfake-detection-challenge/data)
- [arXiv 2020] [The DeepFake Detection Challenge Dataset](https://arxiv.org/abs/2006.07397)
   - consisting of 5K videos featuring two facial modification algorithms

   - a set of specific metrics to evaluate the performance have been defined and two existing models for detecting deepfakes have been tested to provide a reference performance baseline

- [SenseTime] [DeeperForensics-1.0 Dataset](https://liming-jiang.com/projects/DrF1/DrF1.html)
- [CVPR 2020] [DeeperForensics-1.0: A Large-Scale Dataset for Real-World Face Forgery Detection](https://arxiv.org/abs/2001.03024)
   - represents the largest face forgery detection dataset by far, with 60;000 videos constituted by a total of 17.6 million frames, including 50,000 original collected videos and 10,000 manipulated videos
   - fake videos are generated by a newly proposed end-to-end face swapping framework
   
- [Saarland] Video Forensics HQ
     - [arXiv 2020] [Video Forensics HQ: Detecting High-quality Manipulated Face Videos](https://arxiv.org/abs/2005.10360)
     - to be released

## 4. Current Work

### 4.1 Special Artifact-Based

- [CVPRW 2019] [Protecting World Leaders Against Deep Fakes](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Media%20Forensics/Agarwal_Protecting_World_Leaders_Against_Deep_Fakes_CVPRW_2019_paper.pdf)
   - capture the **distinct facial expression and movements of a specific person** use Action Unit (AU)
- [CVPRW 2019] [Exposing DeepFake Videos By Detecting FaceWarping Artifacts](https://arxiv.org/abs/1811.00656)
   - [code](https://github.com/danmohaha/CVPRW2019_Face_Artifacts)
   - improved version: [DSP-FWA](https://github.com/danmohaha/DSP-FWA)
   - current generated face have **limited resolutions** 
- [WIFS 2018] [In Ictu Oculi: Exposing AI Created Fake Videos by Detecting Eye Blinking](https://arxiv.org/abs/1806.02877)
   - [code](https://github.com/danmohaha/WIFS2018_In_Ictu_Oculi)
   - **Lack of eye blinking** in the synthesized videos
- [ICASSP 2019] [EXPOSING DEEP FAKES USING INCONSISTENT HEAD POSES](https://arxiv.org/abs/1811.00661)
   - [code](https://bitbucket.org/ericyang3721/headpose_forensic/src/master/)
   - the  mismatch between the landmarks at center and outer contour of faked faces is revealed as **inconsistent 3D head poses** estimated from **central** and **whole** facial landmarks 
- [TPAMI 2020] [FakeCatcher: Detection of Synthetic Portrait Videos using Biological Signals](https://arxiv.org/abs/1901.02212)
   - **biological signals** hidden in portrait videos can be used as an implicit descriptor of authenticity, because they are **neither spatially nor temporally preserved** in fake content. 
- [WACVW 2019] [Exploiting Visual Artifacts to Expose Deepfakes and Face Manipulations](https://www.semanticscholar.org/paper/Exploiting-Visual-Artifacts-to-Expose-Deepfakes-and-Matern-Riess/3a8939eade51aac810ec89e4b661a7760f31357e#citing-papers)
   - [code](https://github.com/FalkoMatern/Exploiting-Visual-Artifacts)
   - detect each manipulation method according to corresponding artifacts (eye color inconsistency, hard shadow in nose/contour, missing details in teeth, etc.) 
- [ICCVW 2019] [Deepfake Video Detection through Optical Flow Based CNN](http://openaccess.thecvf.com/content_ICCVW_2019/html/HBU/Amerini_Deepfake_Video_Detection_through_Optical_Flow_Based_CNN_ICCVW_2019_paper.html) 
   -  we propose the adoption of **optical flow** fields to exploit possible inter-frame dissimilarities. 
- [IMVOP 2018] [Detection of Deepfake Video Manipulation](https://www.researchgate.net/publication/329814168_Detection_of_Deepfake_Video_Manipulation) 
   - To contribute to a solution, **photo response non uniformity (PRNU) analysis** is tested for its effectiveness at detecting Deepfake video manipulation
- [CVPR 2020] [Face X-ray for More General Face Forgery Detection](https://arxiv.org/abs/1912.13458)
   - We observe that most existing face manipulation methods share a common step: **blending** the altered face into an existing background image. 
   - The face X-ray of an input face image is **a greyscale image** that reveals whether the input image can be decomposed into the blending of two images from different sources. - [arXiv 2020] [DeepFake Detection Based on DiscrepanciesBetween Faces and their Context](https://arxiv.org/abs/2008.12262)
1- [arXiv 2020] [DeepFake Detection Based on DiscrepanciesBetween Faces and their Context](https://arxiv.org/abs/2008.12262)
1- [arXiv 2020] [DeepRhythm: Exposing DeepFakes with Attentional VisualHeartbeat Rhythms](https://arxiv.org/abs/2006.07634)

### 4.2 Novel Network or Module

- [WIFS 2018] [MesoNet: a Compact Facial Video Forgery Detection Network](https://arxiv.org/abs/1809.00888)
   - [code](https://github.com/DariusAf/MesoNet)
   - **MesoNet** exploits features at a **meso-scopic** level leveraging **Inception Module** and **Dilated Convolution**
- [ISITC 2018] [Forensics Face Detection From GANs Using Convolutional Neural Network](https://www.researchgate.net/publication/328744832_Forensics_Face_Detection_From_GANs_Using_Convolutional_Neural_Network)
   - **VGGFace**
- [ICCV 2019] [FaceForensics++: Learning to Detect Manipulated Facial Images](https://arxiv.org/abs/1901.08971)
   - [code](https://github.com/ondyari/FaceForensics)
   - **XceptionNet**
- [ICASSP 2019] [Capsule-forensics: Using Capsule Networks to Detect Forged Images and Videos](https://arxiv.org/abs/1910.12467)
   - [code](https://github.com/nii-yamagishilab/Capsule-Forensics)
   - **Capsule Network**
- [arXiv 2019] [Exploiting Human Social Cognition for the Detection of Fake and Fraudulent Faces via Memory Networks](https://arxiv.org/abs/1911.07844)
   - We propose a **Hierarchical Memory Network (HMN)** architecture, which is able to successfully detect faked faces by utilizing knowledge stored in neural memories as well as visual cues to reason about the perceived face and anticipate its future semantic embeddings. 
- [CVPR 2020] [On the Detection of Digital Face Manipulation](https://arxiv.org/abs/1910.01717)
   - proposed a novel **attention-based layer** to improve classification performance and produce an attention map indicating the manipulated facial regions. 
- [IJCAI 2020] FakeSpotter : A Simple yet Robust Baseline for Spotting AI-Synthesized Fake Faces
   - We propose the first neuron coverage based fake detection approach that monitors the layer-by-layer neuron behaviors in deep FR systems.

### 4.3 Video forensics

- [AVSS 2018] [Deepfake Video Detection Using Recurrent Neural Networks](https://engineering.purdue.edu/~dgueraco/content/deepfake.pdf)
   - CNN (Inception-v3) + **LSTM**
- [CVPR 2019] [Recurrent Convolutional Strategies for Face Manipulation Detection in Videos](https://arxiv.org/abs/1905.00582)
   - CNN (DenseNet) + **bidirectional RNN**
- [CVPRW 2020] [Deepfakes Detection with Automatic Face Weighting](https://arxiv.org/abs/2004.12027)
   - CNN (EfficientNet) + **GRU**
- [MM 2020] [Sharp Multiple Instance Learning for DeepFake Video Detection](https://arxiv.org/abs/2008.04585)
   - Multi-instance learning + Spatial-temporal module
- [arXiv 2020] [Dynamic texture analysis for detecting fake faces in video sequences](https://arxiv.org/abs/2007.15271)

### 4.4 Two Stream

- [CVPRW 2017] [Two-Stream Neural Networks for Tampered Face Detection](https://www.semanticscholar.org/paper/Two-Stream-Neural-Networks-for-Tampered-Face-Zhou-Han/5c04b3178af0cc5f367c833030c118701c210229#paper-header)
   - Face Classification stream (GoogLeNet) + Patch Triplet stream (Steganalysis feature)
- [TIFS 2019] [Attention-Based Two-Stream Convolutional Networks for Face Spoofing Detection](https://ieeexplore.ieee.org/document/8737949)
   - RGB (contain texture details) + MSR (illumination invariant) & Attention-based fusion
- [arXiv 2019] [Complement Face Forensic Detection and Localization with Facial Landmarks](https://arxiv.org/abs/1910.05455)
   - Face landmark + RGB
- [ICASSP 2020] [SSTNet: Detecting Manipulated Faces Through Spatial, Steganalysis and Temporal Features](https://ieeexplore.ieee.org/abstract/document/9053969)
   - Spatial + Steganalysis + Temporal
- [ECCV 2020] [Two-branch Recurrent Network for Isolating Deepfakes in Videos](https://arxiv.org/abs/2008.03412)
   - Frequency + RGB

### 4.5 Auto-encoder

- [arXiv 2018] [ForensicTransfer: Weakly-supervised Domain Adaptation for Forgery Detection](https://arxiv.org/abs/1812.02510)
   - Image reconstruction + Forensic Embedding decoupling
- [BTAS 2019] [Multi-task Learning for Detecting and Segmenting Manipulated Facial Images and Videos](https://arxiv.org/abs/1906.06876)
   - [code](https://github.com/nii-yamagishilab/ClassNSeg)
   - multi-task learning of  classification (real/fake) and  segmentation (locating manipulated regions in images)
- [arXiv 2019] [Towards Generalizable Forgery Detection with Locality-aware AutoEncoder](https://arxiv.org/abs/1909.05999)
   - To bridge generalization gap, in this paper we propose Locality-aware AutoEcoder (LAE), which combines fine-grained representation learning and enforcing locality in a unified frame-work. 
   - A key characteristic of LAE is the **augmented local interpretability**, which could be regularized using **extra pixel wise forgery masks**, in order to learn intrinsic and meaningful forgery representations. 

### 4.6 Frequency Domain

- [arXiv 2019] [Unmasking DeepFakes with simple Features](https://arxiv.org/abs/1911.00686)
   - [code](https://github.com/cc-hpc-itwm/DeepFakeDetection)
   - image -> **[DFT]** -> sinusoidal components of various frequencies -> **[Azimuthal Average]** -> 1D representation of FFT power spectrum -> **[Classifier]** -> Real/Fake
- [ECCV 2020] [Thinking in Frequency: Face Forgery Detectionby Mining Frequency-aware Clues](https://link.springer.com/chapter/10.1007%2F978-3-030-58610-2_6)
   - Frequency-aware Decomposition (FAD) + Local Frequency Statistics (LFS) extracts

### 4.7 Domain Adaptation

- [CVPR 2020] [One-Shot Domain Adaptation For Face Generation](https://arxiv.org/abs/2003.12869)

### 4.8 Metrics Learning

- [Applied Sciences 2020] [Deep fake image detection based on pairwise learning](https://www.mdpi.com/2076-3417/10/1/370)
- [arXiv 2020] [Detecting Deepfakes with Metric Learning](https://arxiv.org/abs/2003.08645)
- [arXic 2020] [Deep Detection for Face Manipulation](https://arxiv.org/abs/2009.05934)

### 4.9 GAN-fake face detection

- [CVPR 2020] [Global Texture Enhancement for Fake Face Detection In the Wild](https://doi.org/10.1109/CVPR42600.2020.00808)
   - propose to introduce **“Gram Block”** into the CNN architecture and propose a novel architecture coined as Gram-Net as shown. The “Gram Block” captures the **global image texture feature** by calculating the **Gram matrix in different semantic level** 
- [WIFS 2019] [AutoGAN: Detecting and Simulating Artifacts in GAN Fake Images](https://arxiv.org/abs/1907.06515)
   - simulate the artifacts produced by the common pipeline shared by several popular GAN models
- [MWSF 2019] [Detecting GAN generated Fake Images using Co-occurrence Matrices](https://arxiv.org/abs/1903.06836)
- [CVPR 2020] [Watch your Up-Convolution: CNN Based Generative Deep Neural Networks are Failing to Reproduce Spectral Distributions](https://arxiv.org/abs/2003.01826)
   - common up-sampling methods,i.e. known as up-convolution or transposed convolution, are causing the inability of such models to reproduce **spectral distributions** of natural training data correctly
- [CVPR 2020] [CNN-generated images are surprisingly easy to spot... for now](https://peterwang512.github.io/CNNDetection/)
   - with careful pre- and post-processing and data augmentation, a standard image classifier trained on only one specific CNN generator is able to generalize surprisingly well to unseen architectures, datasets, and training methods 
- [arXiv 2020] [DeepFake Detection by Analyzing Convolutional Traces](https://arxiv.org/abs/2004.10448)
- [arXiv 2020] [Fighting Deepfake by Exposing the ConvolutionalTraces on Images](https://arxiv.org/abs/2008.04095)
- [arXiv 2020] [CNN Detection of GAN-Generated Face Imagesbased on Cross-Band Co-occurrences Analysis](https://arxiv.org/abs/2007.12909)


