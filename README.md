Bad Smells Detection Repository for Webpage

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
- Does the method have many conditional branches? Yes
- Does the method is excessively large? Yes
- Does the method use many variables? Yes

*Reference: Object-Oriented Metrics in practice. Michele Lanza, Radu Marinescu. (Book)*

**Feature Envy**
- Does the method use directly more than a few attributes of other classes? *Yes*
- Does the method use far more attributes from other classes than its own? *Yes*
- Do the used "foreign" attributes belong to very few other classes? *Yes*

*Reference: Object-Oriented Metrics in practice. Michele Lanza, Radu Marinescu. (Book)*
