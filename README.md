# Mango Leaf Disease Classification 🥭🍂 using CNN, grad-CAM, and Deep feature extraction + KNN/SVM

<h1><b> Summary Report 📑 </b></h1>

This project aims to differentiate among various diseases (multiclass prediction) present in mango leaves. Various machine learning techniques were employed in this project to achieve optimal performance in a model capable of predicting multiple classes.

<h2><b> About the dataset </b></h2>

<h3><b>Description</b></h3>

<ul>
    <li>Type of data: 240x320 mango leaf images.</li>
    <li>Data format: JPG.</li>
    <li>Number of images: 4000 images. Of these, around 1800 are of distinct leaves, and the rest are prepared by zooming and rotating where deemed necessary.</li>
    <li>Diseases considered (classes): Seven diseases, namely Anthracnose, Bacterial Canker, Cutting Weevil, Die Back, Gall Midge, Powdery Mildew, Healthy and Sooty Mould.</li>
    <li>Distribution of instances: Each of the eight categories contains 500 images.</li>
    <li>How data are acquired: Captured from mango trees through the mobile phone camera.</li>
    <li>Data source locations: Four mango orchards of Bangladesh, namely Sher-e-Bangla Agricultural University orchard, Jahangir Nagar University orchard, Udaypur village mango orchard, and Itakhola village mango orchard.</li>
</ul>

For more details, refer to:

Ali, Sawkat; Ibrahim, Muhammad ; Ahmed, Sarder Iftekhar ; Nadim, Md. ; Mizanur, Mizanur Rahman; Shejunti, Maria Mehjabin ; Jabid, Taskeed (2022), “MangoLeafBD Dataset”, Mendeley Data, V1, doi: 10.17632/hxsnvwty3r.1

<h2><b> Solution and results 🧠 </b></h2>

The dataset consists of 4000 images distributed among 8 classes, with a total of 1800 images representing various leaf disease classes. The remaining images are augmented data derived from these classes. Initially, a CNN model was built as a starting point to examine whether the convolutional layers could effectively extract information from the leaf areas.

Also, a Gradient-weighted Class Activation Mapping (grad-CAM) was employed to understand and visualize the crucial regions of an input image that influenced the classification made by the CNN.

The CNN model exhibited strong performance in both training and validation phases. However, it performed poorly with the test data, indicating a need for additional data to generalize and achieve satisfactory interclass differentiation. Consequently, an alternative approach was employed, utilizing a pretrained model (VGG16) for deep feature extraction. This was combined with a baseline model (KNN) and a comparison model (Support Vector Machine).

<h3><b> Results </b></h3>

Finally, the baseline model achieved an accuracy of 82%, whereas the comparison model outperformed with an accuracy of 98%. The confusion matrices of both models are shown in the following figures.

<div style="display: flex; justify-content: space-between;">
    <div style="text-align: center;">        
        <img src="https://raw.githubusercontent.com/EnriqManComp/Mango-Leaf-Disease-Classification/master/KNN.png" alt="KNN Model">
    </div>
    <div style="text-align: center;">        
        <img src="https://raw.githubusercontent.com/EnriqManComp/Mango-Leaf-Disease-Classification/master/SVM.png" alt="SVM Model">
    </div>
</div>

<h2><b> Result Summary 🔍📑<b></h2>
    
<h3><b> GRAD-CAM visualization </b></h3>
    
<div style="display: flex; justify-content: space-between;">
    <div style="text-align: center;">        
        <img src="https://raw.githubusercontent.com/EnriqManComp/Mango-Leaf-Disease-Classification/master/Samples.png" alt="Samples">
    </div>
    <div style="text-align: center;">        
        <img src="https://raw.githubusercontent.com/EnriqManComp/Mango-Leaf-Disease-Classification/master/Superimposition.png" alt="gradCAM">
    </div>
</div>

<h3><b> Model history </b></h3>
    
<div style="display: flex; justify-content: space-between;">
    <div style="text-align: center;">        
        <img src="https://raw.githubusercontent.com/EnriqManComp/Mango-Leaf-Disease-Classification/master/training.png" alt="Model history">
    </div>    
</div>


