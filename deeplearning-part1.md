# Deep Learning

## 1. What is machine learning?
machine learning is a kind of things of scienist
clusters, studies,computer science, math
artificial interligence

First Introduction: File of study that gives computers the ability to learn without 
being explicitly programmed.

google news (cluster)
recommanded systems(advisce the service)
robots

classes
### 1.1 Unsupervised learning


  - Organize computing clusters
  - Social networking analysis
 > links between people
  - Market segmentation
  > different profile of users
  - Generative models
  > give you new data that resemble old data
  >new chairs, features of chairs
 
### 1.2 unsupervised learning algorithms
- Clustering
> ex: K-means
> analyse data and group them
- Anomaly detection
 > Gaussian Models
 >you have data, model of data, give a shape. 
 >bundle, models how it work
- Dimensionality reduction
> Principal Component Analysis
> Auto-encoder
>represent data by point(x,y,z)
>diffrent coordinate
>diminute the dimension
 - Generative models
 > Generative Adversarial Networks
 
### 1.3 supervised learning
**Right Answers Given**
- Housing price prediction
> Regression: Predict
>continuous valued out put
>
- Breast cancer
> Classification
>Discrete valued output

### 1.4 stratigie
Training Set --> Learning Algorithm L
input(x) --> Hypothesis(h) -->Output(y) -->cost-->h

* If output has
> Real values
==> L regression algorithm
> Discrete values
==> L classification algorithm
* Hypothesis/ model/ mapping (h) can be :
> Linenar function :linear regression (regression)
> Logistic function: logistic regression(classification)
> Neural networks

## Regression

### 2.1 linear Regression

Notations: Training set of housing prices
* m = Number of training examples
* x(i) = "input" variable / features of the i<front colore="red">th</front> example
 * y(i) = "output" variable / "target" variable of the ith example
 

> How to choose the parameters

### 2.1.1 Hypothese Representation

- Multiple features (variables)

Notation:
- n = number of features
- x(i) = input(features) of ith training example.
- x(i)(j) = value of features j in ith training example

> Hypothesis function
> 1 variable
> multivariate 

- How do we represent the hypothesis ?
Training set --> Learning Algorithm L

- Linear hypothesis
> How to choose theta prim ?

### 2.1.2 Cost Function

- Gradient Descent for multiple variables
> Hypothesis
>cost function
>goal: minimise 

### 2.1.3 Gradient Descent
- Gradient Descent: intuition
> Some function J(theta_0, theta_1)
> Want to min(theta_0. theta_1) of J(theta_0, theta_1)
>outline:
>> Start with some theta_0, theta_1
>>keep changing theta_0,theta_1 to reduce J
>>until w hopefully end up at a minimum


- Global minimum ?
- Local minimum ?
never sure we have found the best element

> ways to prove that you have a enough good element


- Gradient Descent for linear Regression
> Cost function
>want to find
>outline:
>>Random values
>>Repeat


- Gradient Descent Algorithm

>if alpha is too small, gradient descent can be slow
> if alpha is too large, gradient descent can overshoot the minimum. It may fail to
> converge, or even diverge

### 2.2 Neural Networks

 origins: Algorithms that try to mimic the brain
 > Was very widely used in 80s and early 90s;
 >popularity diminished in late 90s
 >Recent resurgence: State-of-the-art technique for many applications

### 2.2.1 Non-linear Hypothesis

- Non-linear Regression


### 2.2.2 Neurons and the Brain
- The "One learning algorithm" Hypothesis
> auditory cortex learns to see

- Sensor representations in the Brain
> seeing with your tongue
>Human echolocation(Sonar)

### 2.2.3 Model Representation
- Neural Model: Logistic Unit
> Graphical model
>Hypothesis
>Parameters
>>Cost Function ?
>>Learning algorithm ?
>> Activation Function g:
>>linear, sigmoid
>Layer1
>Layer2
>layer3

- a(i)(j) = "activation" of unit i in layer j
- theta(j) = matrix of weights controlling function mapping from layer j to layer j+1
- if network has s(j) units in layer j, s(j+1) units in layer j+1, then theta(j) will be of dimension s(j+1) X [s(j)+1]
<font color=red>*TTT*</font>










# New Features!

  - Import a HTML file and watch it magically convert to Markdown
  - Drag and drop images (requires your Dropbox account be linked)


You can also:
  - Import and save files from GitHub, Dropbox, Google Drive and One Drive
  - Drag and drop markdown and HTML files into Dillinger
  - Export documents as Markdown, HTML and PDF

>>hhhh

> The overriding design goal for Markdown's
> formatting syntax is to make it as readable
> as possible. The idea is that a
> Markdown-formatted document should be
> publishable as-is, as plain text, without
> looking like it's been marked up with tags
> or formatting instructions.

This text you see here is *actually* written in Markdown! To get a feel for Markdown's syntax, type some text into the left window and watch the results in the right.

### Tech

Dillinger uses a number of open source projects to work properly:

* [Angular] - HTML enhanced for web apps!
* [Ace Editor] - awesome web-based text editor
* [markdown-it] - Markdown parser done right. Fast and easy to extend.

And of course Dillinger itself is open source with a [public repository][dill]
 on GitHub.




```sh
$ cd dillinger
$ npm install -d
$ node app
```

For production environments...

```sh
$ npm install --production
$ NODE_ENV=production node app
```




### Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantanously see your updates!

Open your favorite Terminal and run these commands.

First Tab:
```sh
$ node app
```

Generating pre-built zip archives ***for distribution:***
```sh
$ gulp build dist --prod
```
### Docker
Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to build the image.

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version} .
```
This will create the dillinger image and pull in the necessary dependencies. Be sure to swap out `${package.json.version}` with the actual version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```



### Todos

 - Write MORE Tests
 - Add Night Mode

License
----

MIT


**Free Software, Hell Yeah!**
