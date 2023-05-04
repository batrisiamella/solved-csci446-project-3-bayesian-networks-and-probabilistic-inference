Download Link: https://assignmentchef.com/product/solved-csci446-project-3-bayesian-networks-and-probabilistic-inference
<br>



For the third programming assignment, you are going to compare the performance of one exact inference algorithm to one approximate inference algorithm within the context of working with Bayesian networks. For this assignment, you will test your algorithms on five different Bayesian networks of varying sizes and will consider different amounts of evidence. These networks are available on Bayesian Network Repository, which can be found at http://www.bnlearn.com/bnrepository/. Specifications of the networks can also be found using the BIF format. Some information about the format can be found here: http://sites. poli.usp.br/pmr/ltd/Software/Javabayes/Home/index.html.

The five networks you will work with are described here. Note that, while I am providing the BIFformatted files for these networks in D2L/Brightspace, other formats exist on the BN Repository site, any of which you may use.

<ul>

 <li>Alarm Network (medium)

  <ul>

   <li>Number of nodes: 37, Number of edges: 46, Number of parameters: 509</li>

   <li>Average degree: 2.49, Maximum number of parents: 4, Average Markov blanket size: 3.51</li>

  </ul></li>

 <li>Child Network (small to medium)

  <ul>

   <li>Number of nodes: 20, Number of edges: 25, Number of parameters: 230</li>

   <li>Average degree: 1.25, Maximum number of parents: 2, Average Markov blanket size: 3</li>

  </ul></li>

 <li>Hailfinder Network (large)

  <ul>

   <li>Number of nodes: 56, Number of edges: 66, Number of parameters: 2,656</li>

   <li>Average degree: 2.36, Maximum number of parents: 4, Average Markov blanket size: 3.54</li>

  </ul></li>

 <li>Insurance Network (medium)

  <ul>

   <li>Number of nodes: 27, Number of edges: 52, Number of parameters: 984</li>

   <li>Average degree: 3.85, Maximum number of parents: 3, Average Markov blanket size: 5.19</li>

  </ul></li>

 <li>Win95pts Network (large)

  <ul>

   <li>Number of nodes: 76, Number of edges: 112, Number of parameters: 574</li>

   <li>Average degree: 2.95, Maximum number of parents: 7, Average Markov blanket size: 5.92</li>

  </ul></li>

</ul>

For this project, the following steps are required:

<ul>

 <li>Write a design document that outlines the architecture of your software (include a fully explained UML class diagram), design decisions made in implementing your algorithms, and the experimental design for testing the results.</li>

 <li>Process the five networks to be compatible with your Bayesian network implementation. You should use a common format/data structure for your implementation rather than hard-coding the structure in your program.</li>

 <li>Implement variable elimination, capable of working with any ordering for node elimination.</li>

 <li>Implement Gibbs sampling.</li>

 <li>Test your algorithms on the following scenarios, providing the marginal distributions for the indicated variables. For each network, report the marginal distributions under the conditions where no evidence has been applied as well as under the stated evidence conditions.</li>

</ul>

<ol>

 <li>Alarm Network

  <ul>

   <li>Report [HYPOVOLEMIA, LVFAILURE, ERRLOWOUTPUT] (b) Little Evidence: HRBP=HIGH; CO=LOW; BP=HIGH.</li>

  </ul></li>

</ol>

(c) Moderate Evidence: HRBP=HIGH; CO=LOW; BP=HIGH; HRSAT=LOW; HREKG=LOW; HISTORY=TRUE.

<ol start="2">

 <li>Child Network

  <ul>

   <li>Report [Disease]</li>

   <li>Little Evidence: LowerBodyO2=“&lt;5”; RUQO2=“&gt;=12”; CO2Report=“&gt;=7.5”; XrayReport=Asy/Patchy.</li>

   <li>Moderate Evidence: LowerBodyO2=“&lt;5”; RUQO2=“&gt;=12”; CO2Report=“&gt;=7.5”; XrayReport=Asy/Patchy; GruntingReport=Yes; LVHReport=Yes; Age=“11-30 Days”.</li>

  </ul></li>

 <li>Hailfinder Network

  <ul>

   <li>Report [SatContMoist, LLIW]</li>

   <li>Little Evidence: RSFcst=XNIL; N32StarFcst=XNIL; MountainFcst=XNIL; AreaMoDryAir=VeryWet.</li>

   <li>Moderate Evidence: RSFcst=XNIL; N32StarFcst=XNIL; MountainFcst=XNIL; AreaMoDryAir=VeryWet; CombVerMo=Down; AreaMeso_ALS=Down; CurPropConv=Strong.</li>

  </ul></li>

 <li>Insurance Network

  <ul>

   <li>Report [MedCost, ILiCost, PropCost]</li>

   <li>Little Evidence: Age=Adolescent; GoodStudent=False; SeniorTrain=False; DrivQuality=Poor.</li>

   <li>Moderate Evidence: Age=Adolescent; GoodStudent=False; SeniorTrain=False; DrivQuality=Poor; MakeModel=Luxury; CarValue=FiftyThousand; DrivHistory=Zero.</li>

  </ul></li>

 <li>Win95pts Network

  <ul>

   <li>Report [Problem1, Problem2, Problem3, Problem4, Problem5, Problem6] (b) Evidence: Problem1=No_Output.</li>

   <li>Evidence: Problem2=Too_Long.</li>

   <li>Evidence: Problem3=No.(e) Evidence: Problem4=No. (f) Evidence: Problem5=No.</li>

  </ul></li>

</ol>

(g) Evidence: Problem6=Yes.

<ul>

 <li>Write a paper that incorporates the following elements, summarizing the results of your experiments. You should also output the summary statistics on classification accuracy.

  <ol>

   <li>Title and author name</li>

   <li>A brief, one paragraph abstract summarizing the results of the experiments</li>

   <li>Problem statement, including hypothesis, projecting how you expect each algorithm to perform</li>

   <li>Brief description of algorithms implemented</li>

   <li>Brief description of your experimental approach</li>

   <li>Presentation of the results of your experiments</li>

   <li>A discussion of the behavior of your algorithms, combined with any conclusions you can draw</li>

   <li>Summary</li>

   <li>References (you should have at least one reference related to each of the algorithms implemented,a reference to the data sources, and any other references you consider to be relevant)</li>

  </ol></li>

 <li>Create a video that is no longer than 5 minutes long demonstrating the functioning of your code. This video should focus on behavior and not on walking through the code. You need to show input, data structure, and output. How you do this is entirely up to you, but be sure it will convince the grader that your program works.</li>

</ul>