* 目录
    * [week1. Introduction to Data visulization](#Week1-Introduction_to_data_visulization)
    * [week2. Survey of visualization techniques](#Week2-Survey-of-visualization-techniques)
    * [week3. ]
    (#Week3-)








# Week1. Introduction_to_data_visulization

### 1.1 Data visualization


* compare data,information,knowledge and widsom

<img src="./pic/1_1_1.png" width = "480" height = "300" alt="data_visualization" />


    data: 关键字，名词
    inforamtion：客观真理，事实
    knowledge：带有个人态度的内容，包含比较，等
    widsom： 带条件的事实，in...condition 等

&nbsp;

* data visualization in data science

[where is data visualization useful in data science](https://www.menti.com/cwi1vhv27g)

<img src="./pic/1_1_2.png" width = "380" height = "230" alt="data_visualization" />

&nbsp;

* units of data & inforamtion 

<img src="./pic/1_1_3.png" width = "380" height = "230" alt="data_visualization" />

&nbsp;

* Concepts:
    * **Data visualization** refers to the techniques used to communicate data or information by encoding it as visualobjcts (e.g. points, lines or bars) contained in graphics. The goal is to communicate information clearly and efficiently to users. It is one of the steps in data analysis or data science.
    * **information visualization** is the study of (interactive) visual representations of abstract data to reinforce human cognition.

You are aware of just 0.7% of what you experience.

&nbsp;

* Universal Capabilities
    * Typically in less than 1/10s
    * Does not require eye movements
    * Does not require focused attention
    * Color and boundary can be detected preattentively
        * Some color combinations are differentiated by everyone (blue/yellow)
        * Some symbols are understood across cultures(emoj)

----
&nbsp;

### 1.2 Examples and uses

<img src="./pic/1_1_4.png"  width = "400" height = "230" alt="data_visualization" />

&nbsp;

* Design Considerations

<img src="./pic/1_3_1.png" width = "420" height = "280" alt="data_visualization" />

&nbsp;

### 1.3 Tools and software

<img src="./pic/1_4_1.png" width = "420" height = "240" alt="data_visualization" />

<img src="./pic/1_4_2.png"  width = "420" height = "240" alt="data_visualization" />

&nbsp;
&nbsp;
&nbsp;

# Week2. Survey of visualization techniques
&nbsp;

### 2.1 Data
Data is plural (from the latin 'what is given')
Datum is a given piece of data
<br>

* Data types
    * Categorical
        * Nominal:  no natural ordering<br>
             eg., gender, ethnicity, nationality
        * Ordinal:  logical ordering but difference not meaningful 差异没有意义<br>
             eg., levels of happiness, levels of difficulty
    * ( Qualified categorical data 另一种分类方法
        * Binomial      eg., right/left,true/false
        * Dichotomous对立的 eg., hot/cold
            * Vs. non-dichotomous   eg,. Likert Chart)
    * Numerical
        * Ratio:  ordered, differences & boubling meaningful, 0 fixed<br>
             eg., temperature in Kelvin (40=2×20), length, height
        * Intervel:  ordered, differences meaningful, doubling not meaningful, 0 arbitrary<br>
             eg., temperature in Celsius (40≠2×20)/Fahrenheit, dates, locations

* Data Models
    * Conceptual<br>
         Semantic description of data entities and their relations
    * Logical<br>
         Implementation independent data design representation<br>
         eg., entity-relationship diagram
    * Physical<br>
         Implementation dependent details by which data is actually stored (with data types)

* Visualization Reference Model
    <img src="./pic/2_1_1.png" width = "580" height = "300" alt="data_visualization" />
<br>
<br>

### 2.2 Visualization Techniques
1. **Charts**
    * Dots
        * <u>Scatterplot</u>散点图  (2+ variables in Cartesian coordinate)
        * <u>Bubble chart</u>  点图 (3 continuous variables: bubble center (2) and radius (1))
    * Bars
        * <u>Bar chart</u>  (Bar length proportional to continuous variable)
        * <u>Lollipop chart</u> 注重具体高度 (Line length proportional to continuous variable and data point)
    * Bar layouts
        * <u>Coxcomb chart</u>鸡冠花图  (Same angle, radius encodes value, colors different categories. Stacked bar chart with radial layout.)
        * <u>Marimekko chart</u>  (Bar chart where the width encodes relative size. Also called Mekko chart.)
        * <u>Waterfall chart</u>  (Cumulative effects of sequence of positive and negative variations)
        <img src="./pic/2_2_1.png" width = "435" height = "320" alt="data_visualization" />
    * Pies
        * <u>Pie chart</u>  (Exploded pie chart. Pie charts, are a stacked bar charts in polar coordinates. Angle encodes proportion.)
        * <u>Donut chart</u>  (Pie Chart with centre area cut out. Angle encodes proportion.)
        <img src="./pic/2_2_2.png" width = "380" height = "160" alt="data_visualization" />
    * Lines
        * <u>line chart</u> (Trends on continuous variables, e.g., time-series)
        * <u>Sparkline</u>心电图  (Trends on small window size [Tufte 2004])
    * Line layouts
        * <u>Slopegraph</u>  (Shows data values, trends [Tufte 1983])
        * <u>Parallel coordinates</u>  (Multivariate data.)
        * <u>Radar chart</u>  (Multivariate data. Also named web, spider, star, cobweb, polar, or Kiviat.)
        <img src="./pic/2_2_3.png" width = "400" height = "320" alt="data_visualization" />
    * Area
        * <u>Area chart</u>  (Show cumulative or proportions and trends)
        * <u>Steramgraph</u>  (Type of stacked area graph which is displaced around a central axis, resulting in a flowing, organic shape)
        <img src="./pic/2_2_4.png" width = "440" height = "190" alt="data_visualization" />


2. **Graphs and Trees**
    * Hierarchies
        * <u>Dendrogram</u>系统树图  (From Greek dendro tree and gramma drawing.)
        * <u>Reingold-tilford tree</u>  (Hierarchical data as linked tree)
        <img src="./pic/2_2_5.png" width = "440" height = "225" alt="data_visualization" />

        * <u>treemap</u>  (Hierarchical data as nested rectangles. Area proportional to value.)
        * <u>sunburst</u>和鸡冠图很像  (Hierarchical data as rings. Center is root node. Angles are equal or proportional to value.)
    * Flowcharts
        * <u>Alluvial diagram</u> (Shows relations between multivariate data. Named after alluvial fans formed by soil deposited by streaming water.)
        * <u>Sankey Diagram</u>  (Magnitude of flow between nodes in a network)
        <img src="./pic/2_3_6.png" width = "500" height = "225" alt="data_visualization" />
    * <u>Networks network graph</u>  (Relationships (lines) between entities (nodes))
    * Matrix
        * <u>Heat map</u>  (Matrix values as colors)
        * <u>Chord Diagram</u>弦图表  (Shows directed relationships among a group of entities in a matrix)
        <img src="./pic/2_2_7.png" width = "350" height = "170" alt="data_visualization" />

3. **Clouds**
    * <u>Word Cloud</u>
    * <u>Bubble cloud</u>
    * <u>Circle packing</u>圆互相包含  (Bubble cloud technique with hierarchical information as enclosing circles)

4. **Temporal**
    * <u>Time series plot</u>  (Values ordered in time as a line chart)
    * <u>Gantt chart</u>工作日程表  (Schedule with tasks layed out on time axis)
    * <u>Timeline</u>  (Events layed out on time axis)
    <img src="./pic/2_2_8.png" width = "450" height = "250" alt="data_visualization" />

5. **Geospatial and Mapping**
    * Thematic maps主题地图
        * <u>Choropleth</u>等值线图  (Areas are shaded or patterned in proportion to variable)
        * <u>Proportional symbol map</u>  (Scaled symbols show data for areas/locations. Also called Graduated Symbol Map.)
        * <u>Dot map</u>  (Can be used to locate each occurrence of a phenomenon. One-to-one or one-to-many.)
        <img src="./pic/2_2_9.png" width = "500" height = "300" alt="data_visualization" />
        
        * <u>Cartogram</u>统计图  (Area used to display value. Distortion used to show continuous variables)
        * <u>Isopleth</u>等值线  (Use contours等高线 to show continuous variables. Also called Isarithmic.)
        <img src="./pic/2_2_10.png" width = "410" height = "210" alt="data_visualization" />
    * Other named
        * <u>Topographic</u>  (Detailed quantitative representation of land relief using contour lines)
        * <u>Nautical</u>航海的  (Charts of maritime/coastal area)
        * <u>Image based</u>  (Using satellite or aerial imagery)
        <img src="./pic/2_2_11.png" width = "500" height = "300" alt="data_visualization" />

<br>
<br>

### 2.3 Introduction to WEB technologies

<img src="./pic/2_3_1.png" width = "420" height = "240" alt="data_visualization" />

* asynchronous javascript & html (AJAX)

    AJAX是指一种创建交互式、快速动态网页应用的网页开发技术，无需重新加载整个网页的情况下，能够更新部分网页的技术。
    通过在后台与服务器进行少量数据交换，Ajax 可以使网页实现异步更新。这意味着可以在不重新加载整个网页的情况下，对网页的某部分进行更新。


* Web Languages
    * 1. HTML (hypter-text markup language)
            * defines the page semantics or meaning
            * whitespace and line breaks disregarded
            * HTML documnet as a tree of html <u>elements</u> (tag with attributes)
            * two attibures (class & id) used to identify elements
            * elements example : svg
                <img src="./pic/2_3_2.png" width = "420" height = "240" alt="data_visualization" />
    * 2. CSS (Cascading Style Sheets)
            * used to define the appearance of HTML elements
            * including in web pages<br>
                <img src="./pic/2_3_3.png" width = "300" height = "240" alt="data_visualization" />
            * selectors <br>
                div.foo (div elements with <u>class</u> foo)<br>
                div #foo (elements with <u>id</u> foo inside a div) have space before # means inside <br>
                div,.foo (div elements <u>and</u> elements with class foo)<br>
                div p.foo (elemetns with class foo <u>in</u> a p in a div)<br>
    * 3. Javascript
            * implemented in browsers and non-browser, e.g., node
            * uses in browsers<br>
                user interaction<br>
                asynchronous communications<br>
                control the browser<br>
                alter the content<br>
            * including in web pages<br>
                <img src="./pic/2_3_4.png" width = "210" height = "140" alt="data_visualization" />
            * main features
                a. object-oriented language 面向对象
                ```js
                //denotes a comment
                obj = {first: 'Joseph', last: 'Priestley'}; //object literal
                obj.first  //'Joseph'
                ```
                b. everything is mutable可变的
                ```js
                obj = {first: 'Joseph', last: 'Priestley'};
                obj.first = 'Joe'  //now first is 'Joe'
                ```
                c. dynamic typing
                ```js
                //primitive types
                var foo = true;       //Boolean
                var foo = null;       //Null
                var foo = undefined;  //Undefined
                var foo = 2.3;        //Number
                var foo = 'bar'       //String
                ```
                d. function level scope
                ```js
                var b = 5;  //global scope, i.e., at the top of the script
                function f(a) {
                var b = 3;  //local scope, i.e., within the scope of the function
                return a + b;
                }
                b;  //5
                ```
                e. first-calss functions
                ```js
                //functions treated similar to any other variable
                var pi = function() { return Math.PI; }  //assign functions to a variable

                function add(a, f) { return a + f(); }
                add(1, pi);  //pass functions as argument

                function addPi() {
                return function(a) {  //return functions
                    return a + Math.PI;
                }
                }
                ```
            * Hoisting<br>
                Hoisting refers to the moving of variable declarations at the top of their scope when the script is parsed
                <img src="./pic/2_3_5.png" width = "490" height = "240" alt="data_visualization" />
            * Closure<br>
                A closure is the combination of a function and the lexical environment within which that function was declared.
                ```js
                function exampleClosure(arg1, arg2) {  //closure example
                    var localVar = 2;
                    function exampleReturned(innerArg) {  //inner function (declaration)
                        return ((arg1 + arg2) / (localVar + innerArg));
                    }
                    return exampleReturned;  //reference to inner function
                }

                var globalVar = exampleClosure(2, 4);

                console.log(globalVar);  //[Function: exampleReturned]

                globalVar(4);  //1 = ((2 + 4) / (2 + 4))
                ```


&nbsp;
&nbsp;
&nbsp;

# week3. Design space of visualizations, graphing in teh browser, introduction to D3 and Vega
&nbsp;

**Infographics** (a clipped compound of "information" and "graphics") are graphic visual representations of information, data or knowledge intended to present information quickly and clearly. They can improve cognition by utilizing graphics to enhance the human visual system's ability to see patterns and trends.

A **dashboard** is a type of graphical user interface which often provides at-a-glance views of key performance indicators (KPIs) relevant to a particular objective or business process. In other usage, "dashboard" is another name for "progress report" or "report.".


### 3.1 Design space and design trade-offs

### 3.2 Graphing in the browser

### 3.3 Introduction to D3

### 3.4 Introduction to Vega and Vega-lite



