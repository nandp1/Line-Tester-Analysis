# Welcome to Line by Tester Analysis 

  Here we learn on how to conduct Line by Tester analysis which is the most common design used by Plant Breeders to estimate Combining ability and Genetic variances. 


Contents

[Method 1](https://github.com/nandp1/Line-Tester-Analysis/blob/master/README.md#method-1)

##  Setup R for your Computer

R is a programming language and free software used for Statistical computation. 
1. Download and Install the [R base](https://cloud.r-project.org/) package
2. Download and Install the free version of [R Studio](https://rstudio.com/products/rstudio/download/) 



## Method 1 
## By agricolae package 

- Open R Studio and install package called **agricolae** 

```install.packages('agricolae', dependencies=True)
```                                        

- Loading the installed package 

```library(agricolae)
```

There are two Line x Tester dataset in agricole package named as **heterosis** and **LxT**

- Loading dataset **LxT**

```data(LxT)
```

- Understanding the struture of dataset. 

```str(LxT)
```

- If you wish to view entire dataset then

```View(LxT)
```

> There are 5 Lines and 3 Testers. Note that the parental data is mentioned at the end of the dataset. 

- Now using the function `lineXtester` of the agricolae package we perform Line x Tester analysis. 

```output2<-with(LxT,lineXtester(replication, line, tester, yield))
```

> Results is displayed which can be copied and saved. 









