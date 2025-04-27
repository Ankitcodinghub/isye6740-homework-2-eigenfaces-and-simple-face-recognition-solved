# isye6740-homework-2-eigenfaces-and-simple-face-recognition-solved
**TO GET THIS SOLUTION VISIT:** [ISYE6740 Homework 2-Eigenfaces and simple face recognition Solved](https://www.ankitcodinghub.com/product/isye6740-homework-2-eigenfaces-and-simple-face-recognition-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;79600&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;5&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (5 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ISYE6740 Homework 2-Eigenfaces and simple face recognition Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (5 votes)    </div>
    </div>
<h2>1. Eigenfaces and simple face recognition</h2>
This question is a simplified illustration of using PCA for face recognition. We will use a subset of data from the famous Yale Face dataset.

<strong>Remark: </strong>You will have to perform downsampling of the image by a factor of 4 to turn them into a lower resolution image as a preprocessing (e.g., reduce a picture of size 16-by-16 to 4-by-4). In this question, you can implement your own code or call packages.

First, given a set of images for each person, we generate the eigenface using these images. You will treat one picture from the same person as one data point for that person. Note that you will first vectorize each image, which was originally a matrix. Thus, the data matrix (for each person) is a matrix; each row is a vectorized picture. You will find weight vectors to combine the pictures to extract different “eigenfaces” that correspond to that person’s pictures’ first few principal components.

<ul>
<li>&nbsp;Perform analysis on the Yale face dataset for Subject 1 and Subject 2, respectively, usingall the images EXCEPT for the two pictures named subject01-test.gif and subject02-test.gif. <strong>Plot the first 6 eigenfaces for each subject. </strong>When visualizing, please reshape the eigenvectors into proper images. Please explain can you see any patterns in the top 6 eigenfaces?</li>
<li>Now we will perform a simple face recognition task.</li>
</ul>
Face recognition through PCA is proceeded as follows. Given the test image subject01-test.gif and subject02-test.gif, first downsize by a factor of 4 (as before), and vectorize each image. Take the top eigenfaces of Subject 1 and Subject 2, respectively. Then we calculate the <em>projection residual </em>of the 2 vectorized test images with the vectorized eigenfaces:

<em>s<sub>ij </sub></em>= k(test image)<em><sub>j </sub></em>− (eigenface<em><sub>i</sub></em>)(eigenface)<em><sup>T</sup><sub>i </sub></em>(test image)

Report all four scores: <em>s<sub>ij</sub></em>, <em>i </em>= 1<em>,</em>2, <em>j </em>= 1<em>,</em>2<em>. </em>Explain how to recognize the faces of the test images using these scores.

<ul>
<li>(Bonus: 2 points) Explain if face recognition can work well and discuss how we can improve it possibly.</li>
</ul>
<h2>2. Order of faces using ISOMAP</h2>
This question aims to reproduce the ISOMAP algorithm results in the original paper for ISOMAP, J.B. Tenenbaum, V. de Silva, and J.C. Langford, Science 290 (2000) 2319-2323 that we have also seen in the lecture as an exercise (isn’t this exciting to go through the process of generating results for a high-impact research paper!)

The file isomap.mat (or isomap.dat) contains 698 images, corresponding to different poses of the same face. Each image is given as a 64 × 64 luminosity map, hence represented as a vector in R<sup>4096</sup>. This vector is stored as a row in the file. (This is one of the datasets used in the original paper.) In this question, you are expected to implement the ISOMAP algorithm by coding it up yourself. You may find the shortest path (required by one step of the algorithm), using <a href="https://scikit-learn.org/stable/modules/generated/sklearn.utils.graph_shortest_path.graph_shortest_path.html">https://scikit-learn.org/stable/modules/generated/ </a><a href="https://scikit-learn.org/stable/modules/generated/sklearn.utils.graph_shortest_path.graph_shortest_path.html">sklearn.utils.graph_shortest_path.graph_shortest_path.html</a><a href="https://scikit-learn.org/stable/modules/generated/sklearn.utils.graph_shortest_path.graph_shortest_path.html">.</a>

Using Euclidean distance (i.e., in this case, a distance in R<sup>4096</sup>) to construct the -ISOMAP (follow the instructions in the slides.) You will tune the <em>&nbsp;</em>parameter to achieve the most reasonable performance. Please note that this is different from <em>K</em>-ISOMAP, where each node has exactly <em>K </em>nearest neighbors.

<ul>
<li>(10 points) Visualize the nearest neighbor graph (you can either show the adjacency matrix (e.g., asan image), or visualize the graph similar to the lecture slides using graph visualization packages such as Gephi (https://gephi.org) and illustrate a few images corresponds to nodes at different parts of the graph, e.g., mark them by hand or use software packages).</li>
<li>(20 points) Implement the ISOMAP algorithm yourself to obtain a two-dimensional low-dimensionalembedding. Plot the embeddings using a scatter plot, similar to the plots in lecture slides. Find a few images in the embedding space and show what these images look like and specify the face locations on the scatter plot. Comment on do you see any visual similarity among them and their arrangement, similar to what you seen in the paper?</li>
<li>(10 points) Now choose <em>`</em><sub>1 </sub>distance (or Manhattan distance) between images (recall the definition from “Clustering” lecture)). Repeat the steps above. Use -ISOMAP to obtain a <em>k </em>= 2 dimensional embedding. Present a plot of this embedding and specify the face locations on the scatter plot. Do you see any difference by choosing a different similarity measure by comparing results in Part (b) and Part (c)?</li>
<li>(10 points) Perform PCA (you can now use your implementation written in Question 1) on the imagesand project them into the top 2 principal components. Again show them on a scatter plot. Explain whether or you see a more meaningful projection using ISOMAP than PCA.</li>
</ul>
<h2>3. PCA: Food consumption in European countries</h2>
The data food-consumption.csv contains 16 countries in Europe and their consumption for 20 food items, such as tea, jam, coffee, yogurt, and others. We will perform principal component analysis to explore the data. In this question, please implement PCA by writing your own code (you can use any basic packages, such as numerical linear algebra, reading data, in your file).

First, we will perform PCA analysis on the data by treating each country’s food consumption as their “feature” vectors. In other words, we will find weight vectors to combine 20 food-item consumptions for each country.

(a) (5 points) For this problem of performing PCA on countries by treating each country’s food consumption as their “feature” vectors, explain how the data matrix is set-up in this case (e.g., the columns and the rows of the matrix correspond to what). Now extract the first two principal components for each data point (thus, this means we will represent each data point using a two-dimensional vector). Draw a scatter plot of two-dimensional representations of the countries using their two principal components. Mark the countries on the lot (you can do this by hand if you want). Please explain any pattern you observe in the scatter plot.

(c) (5 points) Now, we will perform PCA analysis on the data by treating country consumptions as “feature” vectors for each food item. In other words, we will now find weight vectors to combine country consumptions for each food item to perform PCA another way. Project data to obtain their two principle components (thus, again each data point – for each food item – can be represented using a two-dimensional vector). Draw a scatter plot of food items. Mark the food items on the plot (you can do this by hand if you do not want). Please explain any pattern you observe in the scatter plot.
