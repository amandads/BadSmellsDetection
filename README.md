## Detecting Bad Smells with Machine Learning Algorithms: an Empirical Study ##
### Complementary Webpage ###

### Dataset Download

**Class Level**
- [God Class](https://drive.google.com/open?id=1VRkqyqjKG98COWuhaed-_40vkBDKD8y0)
- [Refused Parent Bequest]

**Method Level**
- [Long Method]
- [Feature Envy]

### List of Systems
- apache-commons-lang
- apache-commons-codec
- apache-commons-io
- apache-commons-logging
- apache-lucene
- checkstyle
- hadoop
- hibernate
- htmlunit
- jasperreports
- jfreechart
- jhotdraw
- jmeter
- quartz
- spring-framework
- squirrelsql
- struts
- tapestry
- tomcat
- weka

### Manual Validation Process
We defined as parameters for the sample size calculation a confidence level of 90%, with error of 10%. With the sample sizes in hand, we extracted from our ground truth the necessary samples for each bad smell. First we randomized the ground truth of each bad smell ten times using different seeds. Second, we randomly extracted the classes and methods that was evaluated without replacement.

To the manual evaluation, we based our strategy on the work of Schumacher et al. We have elaborated three binary question for each bad smell. Also, the respodend could answer with a 'I do not know', in which the answer will being posteriorly discarded from our analysis. We based our questions on the work of Schumacher et al. and Marinescu et al. The samples were distributed for six practioneers in a homogeneous way, assuring that they evaluate samples of the same system and an similar quantity of instances. Each practioneer answered the six questions concerning the class and method in the sample, avoiding the directioning of the desired result. If the evaluator answered two or more questions with positive evidences on the presence of the smell, the instance is classified as smelly. If not, the instance is classified as non-smelly. With results in hands, the agreements between tools and manual validation can be compared. 

### Manual Validation Questions
*The answer after the question defines which answer indicates the presence of Bad Smell.*

**God Class**
- Does the class have more than one responsibility? *Yes*
- Does the class have functionality that would fit better into other classes? *Yes*
- Would splitting up the class improve the overall design? *Yes*

*Reference: Building Empirical Support for Automated Code Smell Detection. Jan Schumacher et al.*

**Refused Parent Bequest**
- Does the class use only a little of parent's behaviour? *Yes*
- Does the parent class provide more than a few protected members? *Yes*
- Does the class is too small/simple? *No*

*Reference: Object-Oriented Metrics in practice. Michele Lanza, Radu Marinescu. (Book)*

**Long Method**
- Does the method have many conditional branches? *Yes*
- Does the method is excessively large? *Yes*
- Does the method use many variables? *Yes*

*Reference: Object-Oriented Metrics in practice. Michele Lanza, Radu Marinescu. (Book)*

**Feature Envy**
- Does the method use directly more than a few attributes of other classes? *Yes*
- Does the method use far more attributes from other classes than its own? *Yes*
- Do the used "foreign" attributes belong to very few other classes? *Yes*

*Reference: Object-Oriented Metrics in practice. Michele Lanza, Radu Marinescu. (Book)*
