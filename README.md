# ce4003-cz4003-computer-vision-solved
**TO GET THIS SOLUTION VISIT:** [CE4003/CZ4003: Computer Vision Solved](https://www.ankitcodinghub.com/product/ce4003-cz4003-computer-vision-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114317&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CE4003\/CZ4003: Computer Vision Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (1 vote)    </div>
    </div>
Lab 1: Point Processing + Spatial Filtering + Frequency Filtering +

Imaging Geometry

1. Objectives

This laboratory aims to introduce image processing in MATLAB context. In this laboratory you will:

a. Become familiar with the MATLAB and Image Processing Toolbox software package.

b. Experiment with the point processing operations of contrast stretching and histogram equalization.

c. Evaluate how different Gaussian and median filters are suitable for noise removal.

d. Become familiar with the frequency domain operations

e. Understand imaging geometry.

2. Experiments

2.1 Contrast Stretching

Obtain the image mrt-train.jpg from the NTULearn website under Course Contents/ Laboratory Material/Images.

a. Input the image into a MATLAB matrix variable by executing:

&gt;&gt; Pc = imread(‘mrt-train.jpg’);

&gt;&gt; whos Pc

The whos command is to show whether the image is read as an RGB or gray-scale image. Notice that this is a 320x443x3 uint8 matrix indicating a colour image with byte values. You will need to convert this into a grayscale image by:

&gt;&gt; P = rgb2gray(Pc);

b. View this image using imshow. Notice that the image has poor contrast. Your initial task will be to investigate different methods for improving the image appearance using point processing. In point processing, the image transformation is carried for each pixel independently of neighbouring pixels.

c. Check the minimum and maximum intensities present in the image:

&gt;&gt; min(P(:)), max(P(:))

Contrast stretching involves linearly scaling the gray levels such the smallest intensity present in the image maps to 0, and the largest intensity maps to 255.

d. Next, write two lines of MATLAB code to do contrast stretching. Hint: This involves a subtraction operation followed by multiplication operation (note that for images which contain uint8 elements, you will need to use imadd, imsubtract, etc. for the arithmetic instead of the usual operators; alternatively you can convert to a double-valued matrix first using double, but you will need to convert back via uint8 prior to using imshow — see below).

Check to see if your final image P2 has the correct minimum and maximum intensities of 0 and 255 respectively by using the min and max commands again.

e. Finally, redisplay the image by

&gt;&gt; imshow(P2);

Note again that if you choose to convert your byte images to doubles first, you will need to use the uint8 command is necessary to convert the P2 double values back to byte values. Otherwise, imshow detects P2 to be double and assumes that the intensity range is between 0.0 and 1.0.

An alternative is to use the imshow as such:

&gt;&gt; imshow(P2,[]);

This does automatic contrast stretching of the display but does not affect the input matrix. This allows you to ignore whether you are displaying byte or double-valued images.

2.2 Histogram Equalization

You will be using the inbuilt command histeq to do histogram equalization. Histogram equalization involves nonlinearly mapping some gray levels to other levels, in order to create a resultant histogram which is approximately uniform.

a. Display the image intensity histogram of P using 10 bins by

&gt;&gt; imhist(P,10);

Next display a histogram with 256 bins. What are the differences?

b. Next, carry out histogram equalization as follows:

&gt;&gt; P3 = histeq(P,255);

Redisplay the histograms for P3 with 10 and 256 bins. Are the histograms equalized? What are the similarities and differences between the latter two histograms?

c. Rerun the histogram equalization on P3. Does the histogram become more uniform? Give suggestions as to why this occurs.

2.3 Linear Spatial Filtering

In linear spatial filtering, typically an input image f(x,y) is convolved with a small spatial filter h(x,y) to create an output image g(x,y),

a b

g x y( , ) =∑∑ f x( −s y, −t h s t) ( , ) = f x y( , )⊗h x y( , )

s=− =−a t b

The function h(x,y) can be considered to be the impulse response of the filter system. Another common name for h(x,y) is the point-spread function (PSF).

a. Generate the following filters:

x +y2

(i) Y and X-dimensions are 5 and σ = 1.0

(ii) Y and X-dimensions are 5 and σ = 2.0

Normalize the filters such that the sum of all elements equals to 1.0. View the filters as 3D graphs by using the mesh function. These filters are Gaussian averaging filters.

b. Download the image ‘ntu-gn.jpg’ from NTULearn and view it. Notice that this image has additive Gaussian noise.

c. Filter the image using the linear filters that you have created above using the conv2 function, and display the resultant images. How effective are the filters in removing noise? What are the trade-offs between using either of the two filters, or not filtering the image at all?

d. Download the image ‘ntu-sp.jpg’ from NTULearn and view it. Notice that this image has additive speckle noise.

e. Repeat step (c) above. Are the filters better at handling Gaussian noise or speckle noise?

2.4 Median Filtering

Median filtering is a special case of order-statistic filtering. For each pixel, the set of intensities of neighbouring pixels (in a neighbourhood of specified size) are ordered. Median filtering involves replacing the target pixel with the median pixel intensity. Repeat steps (b)-(e) in Section 2.3, except instead of using h(x,y) and conv2, use the command medfilt2 with different neighbourhood sizes of 3×3 and 5×5. How does Gaussian filtering compare with median filtering in handling the different types of noise? What are the tradeoffs?

2.5 Suppressing Noise Interference Patterns

Occasionally with poor television reception, parallel lines will be seen on the screen corrupting the desired image. These are interference patterns. Here we explore how bandpass filtering can be used to suppress such interference.

““““““““““““““““““““““““`

a. Download the image ‘pck-int.jpg’ from NTULearn and display it from MATLAB. Notice the dominant diagonal lines destroying the quality of the image.

b. Obtain the Fourier transform F of the image using fft2, and subsequently compute the power spectrum S. Note that F should be a matrix of complex values, but S should be a real matrix. Display the power spectrum by

&gt;&gt; imagesc(fftshift(S.^0.1));

&gt;&gt; colormap(‘default’);

fftshift is used to shift the origin of the Fourier transform to the centre of the image. Note that the origin corresponds to the DC (or zero frequency) component. The power to 0.1 is only used to nonlinearly scale the power spectrum such that it is easier to visualize the frequency components.

Notice that there are two distinct, symmetric frequency peaks that are isolated from the central mass. These frequency components correspond to the interference pattern.

c. Redisplay the power spectrum without fftshift. Measure the actual locations of the peaks. You can read the coordinates off the x and y axes, or you can choose to use the ginput function.

d. Set to zero the 5×5 neighbourhood elements at locations corresponding to the above peaks in the Fourier transform F, not the power spectrum. Recompute the power spectrum and display it as in step (b).

e. Compute the inverse Fourier transform using ifft2 and display the resultant image. Comment on the result and how this relates to step (c). Can you suggest any way to improve this?

f. Download the image `primate-caged.jpg’ from NTULearn which shows a primate behind a fence. Can you attempt to “free” the primate by filtering out the fence? You are not likely to achieve a clean result but see how well you can do.

2.6 Undoing Perspective Distortion of Planar Surface

The goal in this part of the experiment is to take an original slanted view of a book, and compute the projective transformation to warp the image to a frontal view. The final warped image should have the scale 1 pixel (image) = 1 mm (book dimension).

The following paragraph provides the basic knowledge on 2D planar projective transformation. A 2D planar projective transform is expressed via a 3×3 matrix:

kxim  m11 m12 m13X w 

kyim   = m21 m22 m23Yw 

 k   m31 m32 1  1 

where Xw and Yw are the coordinates of a point in the input image, while xim and yim are the coordinates of the transformed point in the output image. This can be alternatively expressed in algebraic form:

m X11 w +m Y12 w +m13 ,yim = m X21 w +m Y22 w +m23 . xim =

m X31 w +m Y32 w +1 m X31 w +m Y32 w +1

X w1



 0

X w2 

 0

 .



 .

X wn 

 0 Yw1

0

Yw2

0

.

.

Ywn

0 1

0

1

0

.

.

1

0 0

X w1

0

X w2

.

.

0

X wn 0

Yw1

0

Yw2

.

.

0

Ywn 0

1

0

1

.

.

0

1 −xim1 X w1

−y Xim1 w1

−x Xim2 w2

−y Xim2 w2

.

.

−x Ximn wn

−y Ximn wn −x Yim1 w1m11 xim1 

−y Yim1 w1m12 yim1 

−x Yim2 w2m13 xim2 

2 2   2 

−y Yim w m21=yim  . (*)

. m22  . 

   

. m23  . 

−x Yimn wn m31 ximn  n n    n  −y Yim w m32 yim 

We can write the above equation in the form of Au = v, where A and v are the 8×8 matrix and 8×1 vector respectively, containing corner data, while u is the 8×1 vector of projective transformation parameters to be computed.

This equation allows the computation of an unknown projective transformation through simple matrix inversion (for 4 correspondences) or pseudo-inversion (for &gt;4 correspondences).

Now please start to go through the following steps.

a. Download `book.jpg’ from the NTULearn website as a matrix P and display the image. The image is a slanted view of a book of A4 dimensions, which is 210 mm x 297 mm.

b. The ginput function allows you to interactively click on points in the figure to obtain the image coordinates. Use this to find out the location of 4 corners of the book, remembering the order in which you measure the corners.

&gt;&gt; [X Y] = ginput(4)

Also, specify the vectors x and y to indicate the four corners of your desired image (based on the A4 dimensions), in the same order as above.

c. Set up the matrices required to estimate the projective transformation based on the equation (*) above.

&gt;&gt; u = A v;

-1

The above computes u = A v, and you can convert the projective transformation parameters to the normal matrix form by

&gt;&gt; U = reshape([u;1], 3, 3)’;

Write down this matrix. Verify that this is correct by transforming the original coordinates

&gt;&gt; w = U*[X’; Y’; ones(1,4)];

&gt;&gt; w = w ./ (ones(3,1) * w(3,:))

Does the transformation give you back the 4 corners of the desired image?

d. Warp the image via

&gt;&gt; T = maketform(‘projective’, U’);

&gt;&gt; P2 = imtransform(P, T, ‘XData’, [0 210], ‘YData’, [0 297]);

e. Display the image. Is this what you expect? Comment on the quality of the transformation and suggest reasons.

3 REPORT

You are expected to write a report towards the end of the semester for coursework grading. The report should be submitted through NTULearn. In the report, (1) Please complete all questions; (2) incorporate the processing results; (3) incorporate the key source codes; and (4) add some comments and analysis if you feel necessary. The complete source code should be in a .m file, to be submitted along with the report.

Because detailed information has been given in this document, the exercises are not very difficult. Please do not copy &amp; paste from your classmates, which can be easily identified.
