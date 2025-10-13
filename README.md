# Galaxy Morphology Classifier
The goal is to build a convolutional neural network that classifies galaxy morphologies (spiral vs elliptical) using Galaxy Zoo data, achieving a considerable accuracy. The repository is to log the learning and creation process. As a Physics undergraduate with only the basics of ML down, the intricate details are brushed aside to make this project more efficient in terms of time and effort. This project is aimed to fulfil the following:

1.Learn to use real astronomical data from citizen science projects and acquire the essential skill of data analysis. 

2.Demonstrate ML skills to potential research supervisors.

3.Foundation for more complex astrophysics ML projects.

# Galaxy Morphological Classification
Galaxies fill the universe with mysterious forms and complex shapes. However, as cryptic as the patterns might be on initial observation, increased availability of data and the advanced technologies providing clearer visualizations of galaxies even from millions of lightyears away has made it possible for scientists to form classifications of them. From these groups, different properties of astrophysical importance like the evolution and formation of galaxies can be predicted. Thus, the aim of classification is not only to group together similar looking galaxies but also increase our physical understanding of them.

Morphological classification is a system that groups galaxies based on their physical appearance e.g their form and shape as seen in images captured by telescopes. Galaxies can be characterized based on certain physical properties like the shape of their centres, the shape and existence of their spirals, their ellipticity, etc.  There are several schemes by which galaxies can be classified according to their morphologies, the most famous being the Hubble sequence, devised by Edwin Hubble and expanded by Gérard de Vaucouleurs and Allan Sandage. However, galaxy classification and morphology are now largely done using computational methods. Another developed method today is the highly successfull method of using crowd-sourced visual inspection (i.e. Galaxy Zoo1 ) to provide quantitative visual morphologies. 

### The Hubble scheme
The Hubble sequence is a morphological classification scheme for galaxies designed by Edwin Hubble. The galxies were divided into three board classes: Ellipticals, Lenticulars and spirals. A fourth class contains galaxies with an irregular appearance. This scheme is the most commonly adopted.

#### Ellipticals 
These galaxies appear as smooth distributions of light in an elliptical form with no prominent features. They are denoted by En, where n is an integer that represents their degree of ellipticity. By convention, 

 $e = 1 - \frac{b}{a}$

where, 
a = semi-major axis length of the ellipse
b = semi-minor axis length of the ellipse

   $n = 10e$

The ellipticity of the galaxy increases with the increase in n, with nearly circular shaped galaxies denoted by E0.

![download](https://github.com/user-attachments/assets/6f30bea0-8473-4476-bb9d-f872124b25d1)
<br>*Giant elliptical galaxy NGC 1316*


#### Lenticulars
Between spiral and elliptical galaxies, lies an intermediate class known as the lenticulars. A bright, central bulge is surrounded by an extended disk-like structure with no spiral structures.
Initially these galaxies were considered as purely hypothetical but with increase in refinement of data showed that Hubble's belief of their existence was a sound one.

#### Spirals
A spiral galaxy consists of a flattened disk, with stars forming a spiral structure, and a central concentration of stars at the bulge. They are denoted by the symbol SB.

![M101_hires_STScI-PRC2006-10a](https://github.com/user-attachments/assets/78cc6b91-c5d7-4f03-bff2-9dd4848232fc)
<br>*The Pinwheel Galaxy (Messier 101/NGC 5457): a spiral galaxy classified as type Scd on the Hubble sequence.*

Almost half of all spirals are also observed to have a bar-like structure, with the bar extending from the central bulge, and the arms begin at the ends of the bar. 

![Hubble2005-01-barred-spiral-galaxy-NGC1300](https://github.com/user-attachments/assets/71189435-2379-46c0-b1bb-2e563ae28878)
<br>*The barred spiral galaxy NGC 1300: a type SBbc*

There are 3 subdivisions for a detailed classification:

<ul>
<li>Sa (SBa) – tightly wound, smooth arms; large, bright central bulge</li>
<li>Sb (SBb) – less tightly wound spiral arms than Sa (SBa); somewhat fainter bulge</li>
<li>Sc (SBc) – loosely wound spiral arms, clearly resolved into individual stellar clusters and nebulae; smaller, fainter bulge</li>
</ul>

Hubble originally described three classes of spiral galaxy. This was extended by Gérard de Vaucouleurs[14] to include a fourth class:
<ul>
<li>Sd (SBd) – very loosely wound, fragmentary arms; most of the luminosity is in the arms and not the bulge</li>
</ul>

