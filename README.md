# cs3353-lab-8--kernels-kernels-kernels-solved
**TO GET THIS SOLUTION VISIT:** [CS3353 Lab 8- Kernels Kernels Kernels Solved](https://www.ankitcodinghub.com/product/aiml-cs-335-solved-14/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;124287&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS3353 Lab 8- Kernels Kernels Kernels Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (2 votes)    </div>
    </div>
Lab 8: Kernels Kernels Kernels

Important: Please read the instructions mentioned in the questions carefully. We have provided boilerplate code for each question. Please ensure that you make changes in the areas marked with TODO. Please read the comments in the code carefully for detailed information regarding input and output format.

1 Trick or Treat

The two moons dataset is a classical set of 2D points that serves as a benchmark for a good classifier. Your task for the first question is to expand the feature space of the input data using polynomial transformations to achieve an accurate decision boundary. This can be using binomial expansion of (x1 + x2)n, where x1 and x2 are the original features and n is a tunable degree. Alternatively, polynomial features for any value of n can be made by designing an appropriate polynomial kernel. Begin by designing additional features in the function poly_features and then design a suitable kernel by completing the function my_kernel.

(a) Two moons dataset (b) Linear Kernel (c) Polynomial kernel

2 Not your typical Kernel

This section aims to help you learn how to apply kernel functions to non linear data so that it can be classified using linear classifiers in an efficient way. More accurately, kernel functions provide a way to manipulate data as though it were projected into a higher dimensional space, by operating on it in its original space. In real life applications data is very segregated and full of complexities like bias, variance, correlation, etc.

So to understand how to best use this data for a task and how it can be used for classification even if the data seems non linearly separable at first glance, we need to understand which kernel function is best suited for a task. For example: In case of 2-D features which are linearly separable, the hyperplane separating them is a flat affine 1D subspace (line). So looking at the below 2 dimensional data find the kernel function which is more likely suited for a support vector classifier.

(a) Sample Data for Kernel 1 (b) Sample Data for Kernel 2 (c) Sample Data for Kernel 3

Try not to overfit to the data and find a kernel function which will generalize well on new data. Fill up the functions Q2_kernel_1, Q2_kernel_2, Q2_kernel_3 such that when they are passed with input feature a shape=(n,d), b shape=(n,d) they return the relation between every point in the higher dimensional space. This can be thought of as getting the relation between input features in higher dimension without converting them into higher dimensional subspace.

3 It’s Convoluted

This section first briefly touches on the idea of convolution for images, used as a backbone in convolution neural networks.

(a) RGB multichannel input with corresponding kernel filter

So the image dimensions can be written as follows: Height (in pixels) * Width (in pixels) * Depth (no. of color channels)

When Depth &gt; 1, then its called a multi input channel.

3.1 Kernel Convolution

This is the process where we simply pass a kernel/filter (matrix of numbers) over the image pixel matrix and transform it based on the kernel values. We discuss the following notations here.

Padding

As we move our filter over our image, it impacts the pixels located on the boundaries much less as compared to the image center. Hence this can be treated as a lossy compression. We thus use padding, usually consisting of zeroes. If we try this with our grey-scale image from before, then it would look like so as in Fig. 4a

Stride It controls how much we move our filter in each step. In this example we take a stride of value = 2, resulting in a final feature map of dimensions 2×2. Fig. 4b, Fig 4c

(a) Padding Instance (b) Convolution using stride=2 (c) Feature Map obtained

By considering the below notations,

• n: image size

• f: filter size

• nc — number of color channels in the image

• p: padding size

• s: stride size

• nf: number of filters we can compute the new dimensions can be calculated by using the following formula:

.

If we then have multiple color channels, i.e. a depth greater than 1, then we can use the following formula to calculate the dimensions:

3.2 Gram Matrix Computation

Given the matrix X, the Gram Matrix is simply given by XT.X.

Upon performing the above convolution, we take nc feature vectors(flattened) from a convolutional feature map of depth nc and compute the dot product with every one of them(including with a feature vector itself). The result is the Gram Matrix. You can read more in detail here –

TODO: Perform the convolution of a given input image pixel array by implementing a naive convolution function.

Then use the feature output obtained above to compute the gram matrix.

(a) Gram Matrix computation post convolu-

tion

4 On the Edge

This section is intended to introduce you to convolution operation by applying it to detect edges in an image. This part requires minimal coding!

A colour image is an array of dimension N x M x 3 where N is the height (number of rows), M is the width (number of columns) and 3 is related to the colors red, green, blue composing the image. A grayscale image image is an array of dimension N x M.

The Sobel operator is used in image processing and computer vision, particularly within edge detection algorithms where it creates an image emphasising edges. Technically, it is a discrete differentiation operator, computing an approximation of the gradient of the image intensity function. At each point in the image, the result of the Sobel–Feldman operator is either the corresponding gradient vector or the norm of this vector. The Sobel–Feldman operator is based on convolving the image with a small, separable, and integer-valued filter in the horizontal and vertical directions and is therefore relatively inexpensive in terms of computations. Please refer to Sobel operator’s (or filter’s) Wikipedia page for more information (recommended).

TO DO: Complete the edgeDetection function in the sections marked. Running the code will save an image called imageWithEdges.png. You are expected to submit that as a part of the submission folder too.

Submission instructions

Complete the functions in assignment.py. Keep the file in a folder named &lt;ROLL_NUMBER&gt;_L8 and compress it to a tar file named &lt;ROLL_NUMBER&gt;_L8.tar.gz using the command tar -zcvf &lt;ROLL_NUMBER&gt;_L8.tar.gz &lt;ROLL_NUMBER&gt;_L8

Submit the tar file on Moodle.

The directory structure should be –

&lt;ROLL_NUMBER&gt;_L8

| – – – – assignment.py

| – – – – Q1.py

| – – – – Q2.py

| – – – – Q3.py

| – – – – Q4.py

| – – – – utils.py

| – – – – input/* Do Not Modify the input directory

| – – – – output/

| – – – – – – – – – imageWithEdges.png

| – – – – – – – – – q1_linear.png

| – – – – – – – – – q1_poly.png

Replace ROLL_NUMBER with your own roll number. If your Roll number has alphabets, they should be in “small” letters.
