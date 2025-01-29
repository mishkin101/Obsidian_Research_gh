<%"---"%>
aliases: 
  - Interpretable machine learning Fundamental principles and 10 grand challenges
  - rudinInterpretableMachineLearning2022
<%"---"%>
<%*
    let citekey = "rudinInterpretableMachineLearning2022"; 
    let date = tp.date.now("YYYY-MM-DD");
    await tp.file.rename(`${citekey}_Analysis`);
%>


##  <h1 class="color-red">Definitions</h>
- <mark class="hltr-red">"case-based reasoning"</mark>  [Page ](zotero://open-pdf/library/items/FYF7GDU4?page=&annotation=4X946TPU) #Further-exploration-needed, #definition

	- define and find examples #Further-exploration-needed, #definition
- <mark class="hltr-red">"disentanglement of neural networks"</mark>  [Page ](zotero://open-pdf/library/items/FYF7GDU4?page=&annotation=DKFSZ6PY) #Further-exploration-needed, #definition

	- define disentanglement #Further-exploration-needed, #definition
- <mark class="hltr-red">"generative or causal constraints"</mark>  [Page ](zotero://open-pdf/library/items/FYF7GDU4?page=&annotation=REY5CCYY) #actionitem, #definition

	- find examples and define #actionitem, #definition
- <mark class="hltr-red">"“Rashomon set”"</mark>  [Page ](zotero://open-pdf/library/items/FYF7GDU4?page=&annotation=2SKICXV2) #actionitem, #important, #definition

	- Define #actionitem, #important, #definition
- <mark class="hltr-red">"Interpretable predictive models, which are constrained so that their reasoning processes are more understandable to humans"</mark>  [Page 2](zotero://open-pdf/library/items/FYF7GDU4?page=2&annotation=9TV29SCN) #Interpretable-machine-learning, #Further-exploration-needed, #definition

	- high level defintion of interpretability the paper uses as basis for defintion. Could refine further #Interpretable-machine-learning, #Further-exploration-needed, #definition
- <mark class="hltr-red">"“Clever Hans” phenomenon"</mark>  [Page 2](zotero://open-pdf/library/items/FYF7GDU4?page=2&annotation=Y7Z5ZL8S) #actionitem, #important, #blackbox, #definition

	- Need to define in relation to impact of using black box models in practice #actionitem, #important, #blackbox, #definition
- <mark class="hltr-red">"underlying distribution of data changes (called domain shift"</mark>  [Page 2](zotero://open-pdf/library/items/FYF7GDU4?page=2&annotation=MVGFEPEC) #Interpretable-machine-learning, #actionitem, #definition

	- define domain shift, and whether thee are generalize frameworks for how this arises in 2-3 key domains were interperetability has a huge effect. #Interpretable-machine-learning, #actionitem, #definition
- <mark class="hltr-red">"Clean” means that the data do not have too much noise or systematic bias"</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=SHSC968Q) #definition
- <mark class="hltr-red">"Tabular” means that the features are categorical or real,"</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=5UKBRRZY) #definition
- <mark class="hltr-red">"Raw” data is unprocessed and has a complex data type"</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=YD5I9DWL) #definition
- <mark class="hltr-red">"soft and hard interpretability constraints"</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=BQA2395E) #Interpretable-machine-learning, #Further-exploration-needed, #definition

	- define differences #Interpretable-machine-learning, #Further-exploration-needed, #definition
- <mark class="hltr-red">"This definition might require refinement, sometimes over multiple iterations with domain experts. There are many papers detailing these issues, the earliest dating from the mid-1990s [e.g., 157]."</mark>  [Page 5](zotero://open-pdf/library/items/FYF7GDU4?page=5&annotation=AMPYWYWH) #Interpretable-machine-learning, #important, #Further-exploration-needed, #definition

	- What drives the definition of interpertabilitiy from a domain level and from the CS community? #Interpretable-machine-learning, #important, #Further-exploration-needed, #definition
- <mark class="hltr-red">"Interpretability penalties or constraints can include sparsity of the model, monotonicity with respect to a variable, decomposibility into sub-models, an ability to perform case-based reasoning or other types of visual comparisons, disentanglement of certain types of information within the model’s reasoning process, generative constraints (e.g., laws of physics), preferences among the choice of variables, or any other type of constraint that is relevant to the domain"</mark>  [Page 5](zotero://open-pdf/library/items/FYF7GDU4?page=5&annotation=7WG3E7LH) #Interpretable-machine-learning, #important, #Further-exploration-needed, #definition

	- Need to understand why knowledge of these penalizes the outcome from (*) #Interpretable-machine-learning, #important, #Further-exploration-needed, #definition
- <mark class="hltr-red">"coring systems are linear classification models that require users to add, subtract, and multiply only a few small numbers in order to make a prediction."</mark>  [Page 16](zotero://open-pdf/library/items/FYF7GDU4?page=16&annotation=CZCFM8UG) #definition, #logical-model
- <mark class="hltr-red">"Case-based reasoning is a paradigm that involves solving a new problem using known solutions to similar past problems [1]. It is a problem-solving strategy that we humans use naturally in our decision-making processes [219]"</mark>  [Page 25](zotero://open-pdf/library/items/FYF7GDU4?page=25&annotation=GLY6YGDE) #definition, #case-based-reasoning
- <mark class="hltr-red">"Nearest neighbor-based techniques. These techniques make a decision for a previously unseen test instance, by finding training instances that most closely resemble the particular test instance"</mark>  [Page 26](zotero://open-pdf/library/items/FYF7GDU4?page=26&annotation=MU57BMYL) #definition, #case-based-reasoning
- <mark class="hltr-red">"Given a previously unseen test instance, they make a decision by finding prototypical cases (instead of training instances from the entire training set) that most closely resemble the particular test instance"</mark>  [Page 27](zotero://open-pdf/library/items/FYF7GDU4?page=27&annotation=FLRVILJY) #definition, #case-based-reasoning
- <mark class="hltr-red">"Disentanglement” here refers to the way information travels through the network: we would perhaps prefer that all information about a specific concept (say “lamps”) traverse through one part of the network while information about another concept (e.g., “airplane”) traverse through a separate part."</mark>  [Page 31](zotero://open-pdf/library/items/FYF7GDU4?page=31&annotation=XJXAPNYM) #definition, #disentanglement
- <mark class="hltr-red">"n general, a PINN is a neural network that approximates the solution of a set of PDEs with initial and boundary conditions. The training of a PINN minimizes the residuals from the PDEs as well as the residuals from the initial and boundary conditions."</mark>  [Page 46](zotero://open-pdf/library/items/FYF7GDU4?page=46&annotation=CN29XNSA) #definition, #physics-machine-learning

	- constraints based on laws of nature, PDE/ODES for material science, etc. #definition, #physics-machine-learning
- <mark class="hltr-red">"The Rashomon effect occurs when there are multiple descriptions of the same event [41] with possibly no ground truth"</mark>  [Page 48](zotero://open-pdf/library/items/FYF7GDU4?page=48&annotation=7R89QVFH) #definition, #Rashomon-Set
- <mark class="hltr-red">"computing statistics of the Rashomon set in parameter space, such as the volume in parameter space, which is called the Rashomon volume"</mark>  [Page 51](zotero://open-pdf/library/items/FYF7GDU4?page=51&annotation=N38NV5AP) #definition, #Rashomon-Set

##  <h1 class="color-orange">Applications</h>

##  <h1 class="color-yellow">Technical Details</h>
- <mark class="hltr-yellow">"min  f ∈F  1 n  ∑  i  Loss(f, zi) + C · InterpretabilityPenalty(f ), subject to (*)  InterpretabilityConstraint(f )"</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=NB3Y9DVT) #Interpretable-machine-learning, #formula

	- We choose a loss function (goal, quanitity/outcome to control) and select a model from a function class as defined by Table 1(?). 

If we increase the interpretability, we must assign a penalty for knowing the reasoning process.

The constraints are domain dependent. #Interpretable-machine-learning, #formula
- <mark class="hltr-yellow">"(xi, yi), xi ∈ Rp, yi ∈ {−1, 1}"</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=TA2C6Q8V) #example

	- Example of data input and assigned label for supervised data item. In relation to (*) #example
- "<mark class="hltr-yellow">"C trades off between accuracy and the interpretability penalty"</mark>" [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=J7NTYF2N)

	- modulates the outcome-- need subjectivity. 
- <mark class="hltr-yellow">"accuracy, weighted accuracy, precision, average precision, precision@N, recall, recall@N, DCG, NCDG, AUC, partial AUC, mean-timeto-failure, etc."</mark>  [Page 5](zotero://open-pdf/library/items/FYF7GDU4?page=5&annotation=FAS5U4WP) #Interpretable-machine-learning, #performance-metrics

	- metrics for performance. Int. has similar taxology. #Interpretable-machine-learning, #performance-metrics
- <mark class="hltr-yellow">"sparsity is measured by the number of leaves in the tree"</mark>  [Page 14](zotero://open-pdf/library/items/FYF7GDU4?page=14&annotation=N6M2JBNS) #formula, #sparsity
- <mark class="hltr-yellow">"g(E[y]) = β0 + f1(x·1) + ... + fp(x·p),"</mark>  [Page 21](zotero://open-pdf/library/items/FYF7GDU4?page=21&annotation=BS7FL9WH) #formula

	- generative additive model #formula
- <mark class="hltr-yellow">"fj (x·j ) =  ∑  thresholdsj′  cj,j′ 1[x·j &gt; θj′ ]."</mark>  [Page 23](zotero://open-pdf/library/items/FYF7GDU4?page=23&annotation=BU3TANNQ) #Generalized-Additive-Model, #equation

	- sum of component functions. #Generalized-Additive-Model, #equation
- <mark class="hltr-yellow">"During training, if the training example’s class agrees with the nearest prototype’s class, then the prototype is moved closer to the training example; otherwise the prototype is moved further away from the training example."</mark>  [Page 27](zotero://open-pdf/library/items/FYF7GDU4?page=27&annotation=DSKALA5Y) #example, #case-based-reasoning

	- method for how prototype reasoning works #example, #case-based-reasoning
- <mark class="hltr-yellow">"he derivative g′(t) with respect to input t (at each of those finitely many points t used for training) is found by leveraging the existing network structure of g using back-propagation"</mark>  [Page 46](zotero://open-pdf/library/items/FYF7GDU4?page=46&annotation=YB68NZ9X) #physics-machine-learning, #method
- <mark class="hltr-yellow">"R(F , f ∗, ) = {f ∈ F such that Loss(f ) ≤ Loss(f ∗) + },"</mark>  [Page 49](zotero://open-pdf/library/items/FYF7GDU4?page=49&annotation=QAH3UA9R) #formula, #Rashomon-Set

##  <h1 class="color-green">Conceptual</h>
- <mark class="hltr-green">"Black box predictive models, which by definition are inscrutable, have led to serious societal problems that deeply affect health, freedom, racial bias, and safety."</mark>  [Page 2](zotero://open-pdf/library/items/FYF7GDU4?page=2&annotation=L5KACVJW) #blackbox, #supportingevidence, #Further-exploration-needed
- <mark class="hltr-green">"black box machine learning model is a formula that is either too complicated for any human to understand, or proprietary"</mark>  [Page 2](zotero://open-pdf/library/items/FYF7GDU4?page=2&annotation=I8SRNF7V) #supportingevidence
- <mark class="hltr-green">"individuals may have been subjected to years of extra prison time due to typographical errors"</mark>  [Page 2](zotero://open-pdf/library/items/FYF7GDU4?page=2&annotation=PTIGNX78) #blackbox, #supportingevidence
- <mark class="hltr-green">"poorly-designed proprietary models for air quality have had serious consequences for public safety during wildfires"</mark>  [Page 2](zotero://open-pdf/library/items/FYF7GDU4?page=2&annotation=J5WZFKVB) #blackbox, #supportingevidence
- <mark class="hltr-green">"Explaining black boxes, rather than replacing them with interpretable models, can make the problem worse by providing misleading or false characterizations"</mark>  [Page 2](zotero://open-pdf/library/items/FYF7GDU4?page=2&annotation=4ZF8ZIK3) #blackbox, #supportingevidence
- <mark class="hltr-green">"one would explain a black box without consideration of whether there is an interpretable model of the same accuracy"</mark>  [Page 3](zotero://open-pdf/library/items/FYF7GDU4?page=3&annotation=4LYI9PTB) #supportingevidence, #Further-exploration-needed

	- In what areas is this becoming an increasing need?


What are some common themes among black box papers that lead to poor explainability ? #supportingevidence, #Further-exploration-needed
- <mark class="hltr-green">"Creating interpretable models can sometimes be much more difficult than creating black box models for many different reasons including:"</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=R4ZYIWGB) #Interpretable-machine-learning, #counterargument

	- depends on model complexity (constraints), data processing leading to deployement slowdowns, uncertainity on definition of interpertability #Interpretable-machine-learning, #counterargument
- <mark class="hltr-green">"here is no scientific evidence for a general tradeoff between accuracy and interpretability when one considers the full data science process for turning data into knowledge."</mark>  [Page 6](zotero://open-pdf/library/items/FYF7GDU4?page=6&annotation=RKMSW8CA) #Interpretable-machine-learning, #critique
- <mark class="hltr-green">"The story of COMPAS is a key example simultaneously demonstrating many pitfalls of black boxes in practice. And, it shows an example of when black boxes are unnecessary, but used anyway."</mark>  [Page 7](zotero://open-pdf/library/items/FYF7GDU4?page=7&annotation=ZPSHA6FD) #blackbox, #supportingevidence
- <mark class="hltr-green">"ar domain is that of Afnan et al. [4], who discuss in vitro fertilization (IVF). In modern IVF, black box models that have not been subjected to randomized controlled trials determine who comes into existence"</mark>  [Page 7](zotero://open-pdf/library/items/FYF7GDU4?page=7&annotation=86SD2DYE) #blackbox, #supportingevidence

	- very morally touchy subject. Relate to randomization and fairness #blackbox, #supportingevidence
- <mark class="hltr-green">"shared decision-making with patients"</mark>  [Page 7](zotero://open-pdf/library/items/FYF7GDU4?page=7&annotation=ZRMMJMKP) #blackbox, #supportingevidence
- <mark class="hltr-green">"“Who is accountable when the model causes harm?”"</mark>  [Page 7](zotero://open-pdf/library/items/FYF7GDU4?page=7&annotation=RBBCWA4L) #blackbox, #supportingevidence
- <mark class="hltr-green">"In these domains, neural networks generally find no advantage."</mark>  [Page 8](zotero://open-pdf/library/items/FYF7GDU4?page=8&annotation=IJTHFINA) #blackbox, #critique

	- relate to rashomon set. Tabular data has good performance without blackbox methods. What would necessitate the trade off to obfsucate interpretability to choose a blackbox model? #blackbox, #critique
- "<mark class="hltr-green">"In such cases, as discussed earlier and in Challenges 4 and 5, interpretable neural networks suffice, without losing accuracy."</mark>" [Page 8](zotero://open-pdf/library/items/FYF7GDU4?page=8&annotation=4SXVYDWY)

	- there is no dichotomy (principle 3)- this is all dependent on the existence of the Rashomon set. Interpretable black box models could exist, and it may be dependent on the type of data the model is deployed on. (tabular vs. raw data). 
- <mark class="hltr-green">"uch issues with explanations have arisen with assessment of fairness and variable importance [258, 82] as well as uncertainty bands for variable importance [113, 97]"</mark>  [Page 10](zotero://open-pdf/library/items/FYF7GDU4?page=10&annotation=JLRSFSQZ) #question, #Interpretable-machine-learning, #critique, #Explainability

	- What are uncertainty bands? #question, #Interpretable-machine-learning, #critique, #Explainability
- <mark class="hltr-green">"posthoc explanation, called saliency maps"</mark>  [Page 10](zotero://open-pdf/library/items/FYF7GDU4?page=10&annotation=YEJAD72D) #critique, #Explainability

	- posthoc processing is not good #critique, #Explainability
- <mark class="hltr-green">"Typographical errors in input data are a prime example of this issue"</mark>  [Page 10](zotero://open-pdf/library/items/FYF7GDU4?page=10&annotation=V9HEKUR4) #blackbox, #critique
- "<mark class="hltr-green">"an interpretable model is constrained, following a domain-specific set of constraints that make reasoning processes understandable."</mark>" [Page 11](zotero://open-pdf/library/items/FYF7GDU4?page=11&annotation=WSW3XDP2)
- "<mark class="hltr-green">"When would we use logical models? Logical models are usually an excellent choice for modeling categorical data with potentially complicated interaction terms"</mark>" [Page 12](zotero://open-pdf/library/items/FYF7GDU4?page=12&annotation=46F97PA8)
- <mark class="hltr-green">"These greedy methods for building decision trees create trees from the top down and prune them back afterwards. They do not go back to fix a bad split if one was made. Consequently, the trees created from these greedy methods tend to be both less accurate and less interpretable than necessary"</mark>  [Page 12](zotero://open-pdf/library/items/FYF7GDU4?page=12&annotation=9PN2WKHT) #Interpretable-machine-learning, #supportingevidence, #data-type, #logical-model

	- relate to table 2 ,data types and models. this if for multiclass data and categorical data #Interpretable-machine-learning, #supportingevidence, #data-type, #logical-model
- <mark class="hltr-green">"This gap can cause a problem in practice because one does not know whether poor performance is due to the choice of model form (the choice to use a decision tree of a specific size) or poor optimization (not fully optimizing over the set of decision trees of that size)."</mark>  [Page 13](zotero://open-pdf/library/items/FYF7GDU4?page=13&annotation=RAIWVI7C) #logical-model
- <mark class="hltr-green">"Can we improve the scalability of optimal sparse decision trees?"</mark>  [Page 14](zotero://open-pdf/library/items/FYF7GDU4?page=14&annotation=BAUI2ZXP) #important, #logical-model

	- accuracy and sparsity are two challenging areas for decision trees #important, #logical-model
- <mark class="hltr-green">"Can we efficiently handle continuous variables?"</mark>  [Page 15](zotero://open-pdf/library/items/FYF7GDU4?page=15&annotation=S4L2Y9JA) #important, #logical-model
- <mark class="hltr-green">"These methods are unable to jointly optimize the selection of variables to split at each internal tree node, the splitting threshold of that variable (if it is continuous), and the tree structure (the overall shape of the tree). Lin et al"</mark>  [Page 15](zotero://open-pdf/library/items/FYF7GDU4?page=15&annotation=YJUIZH3W) #important, #logical-model
- <mark class="hltr-green">"Can we handle constraints more gracefully?"</mark>  [Page 16](zotero://open-pdf/library/items/FYF7GDU4?page=16&annotation=C67VD4GP) #important, #logical-model
- <mark class="hltr-green">"Each scoring system was created using a different method involving different heuristics. Some of them were built using domain expertise alone without data, and some were created using rounding heuristics for logistic regression coefficients and other manual feature selection approaches to obtain integer-valued point scores [see, e.g., 175]."</mark>  [Page 17](zotero://open-pdf/library/items/FYF7GDU4?page=17&annotation=SYX3N3KW) #critique, #logical-model
- <mark class="hltr-green">"When rounding, we lose all signal coming from all variables except the first two. The contribution from the eliminated variables may together be significant even if each individual coefficient is small, in which case, we lose predictive performance."</mark>  [Page 18](zotero://open-pdf/library/items/FYF7GDU4?page=18&annotation=QZVFCGIX) #critique, #logical-model
- <mark class="hltr-green">"1 regularization does more than make the solution sparse, it also imposes a strong 1 bias."</mark>  [Page 18](zotero://open-pdf/library/items/FYF7GDU4?page=18&annotation=56NFXGVB) #critique, #logical-model
- <mark class="hltr-green">"Some of these constraints may be able to be placed into the mathematical program, but it is still not clear whether the solution of the optimization problem one solves would actually be close to the solution of the optimization problem we actually care about."</mark>  [Page 19](zotero://open-pdf/library/items/FYF7GDU4?page=19&annotation=DLINRWWL) #critique, #logical-model
- <mark class="hltr-green">"Improve the scalability of optimal sparse scoring systems: As discussed, for scoring systems, the only practical approaches that produce optimal scoring systems require a MIP solver, and these approaches may not be able to scale to large problems, or optimally handle continuous variables"</mark>  [Page 20](zotero://open-pdf/library/items/FYF7GDU4?page=20&annotation=VQ368IK3) #logical-model, #solution

	- solutions #logical-model, #solution
- <mark class="hltr-green">"Improve the scalability of optimal sparse scoring systems: As discussed, for scoring systems, the only practical approaches that produce optimal scoring systems require a MIP solver, and these approaches may not be able to scale to large problems, or optimally handle continuous variables."</mark>  [Page 20](zotero://open-pdf/library/items/FYF7GDU4?page=20&annotation=IH5RG3DF) #logical-model, #challenge
- <mark class="hltr-green">"Ease of constraint elicitation and handling:"</mark>  [Page 20](zotero://open-pdf/library/items/FYF7GDU4?page=20&annotation=2BU86P2I) #Rashomon-Set, #logical-model
- <mark class="hltr-green">"For instance, if we had better ways of representing and exploring the Rashomon set (see Challenge 9), domain experts might be able to search within it effectively, without fear of leaving that set and producing a suboptimal model."</mark>  [Page 20](zotero://open-pdf/library/items/FYF7GDU4?page=20&annotation=M6TGLWIP) #Rashomon-Set, #logical
- <mark class="hltr-green">"importance of features, we should be able to incorporate that through regularization [307]."</mark>  [Page 21](zotero://open-pdf/library/items/FYF7GDU4?page=21&annotation=79ZY87JP) #logical-model
- "<mark class="hltr-green">"Fig 4. Hierarchical relationships between GAMs, additive models, linear models, and scoring systems."</mark>" [Page 22](zotero://open-pdf/library/items/FYF7GDU4?page=22&annotation=QEAUTEWT)
- <mark class="hltr-green">"sparsity in the number of component functions and smoothness of the component functions"</mark>  [Page 23](zotero://open-pdf/library/items/FYF7GDU4?page=23&annotation=3PIXXEDZ) #important, #Generalized-Additive-Model

	- Main ways to control GAM interpetability #important, #Generalized-Additive-Model
- <mark class="hltr-green">"1 regularization imposes a strong unintended bias on the coefficients when aiming for very sparse solutions. (2) Lou et al. [195] find that imposing smoothness may come at the expense of accuracy, (3)"</mark>  [Page 24](zotero://open-pdf/library/items/FYF7GDU4?page=24&annotation=98M9GWZQ) #important, #Generalized-Additive-Model

	- main issue with regularization and accuracy again #important, #Generalized-Additive-Model
- <mark class="hltr-green">"GAMs are often used on raw medical records or other complex data types, and these datasets are likely to benefit from troubleshooting."</mark>  [Page 24](zotero://open-pdf/library/items/FYF7GDU4?page=24&annotation=KN5GPSZ5) #data-type, #Generalized-Additive-Model

	- model used for raw data type. good at finding patterns in data or missing relationships. Broadest class that can be distilled down into morte speciifc models like decisons trees or scoring systems by controlling sparsity, monotonicity, and smoothness #data-type, #Generalized-Additive-Model
- <mark class="hltr-green">"case-based reasoning applies to both tabular and raw data, including computer vision."</mark>  [Page 25](zotero://open-pdf/library/items/FYF7GDU4?page=25&annotation=3A4S9C6Q) #supportingevidence, #case-based-reasoning
- <mark class="hltr-green">"There are, in general, two types of case-based reasoning techniques: (i) nearest neighbor-based techniques, and (ii) prototype-based techniques"</mark>  [Page 25](zotero://open-pdf/library/items/FYF7GDU4?page=25&annotation=K2IVJ29V) #case-based-reasoning, #methods
- <mark class="hltr-green">"those techniques often require a substantial amount of distance computations (e.g., to find out the nearest neighbors of a test input), which can be slow in practice. Also, it is possible that the nearest neighbors may not be particularly good representatives of a class, so that reasoning about nearest neighbors may not be interpretable"</mark>  [Page 27](zotero://open-pdf/library/items/FYF7GDU4?page=27&annotation=8A3NQA4X) #critique, #case-based-reasoning
- <mark class="hltr-green">"Part-based prototypes. One issue that arises with both nearest neighbor and prototype techniques is the comparison of a whole observation to another whole observation."</mark>  [Page 27](zotero://open-pdf/library/items/FYF7GDU4?page=27&annotation=R3WRI2MN) #critique, #case-based-reasoning
- <mark class="hltr-green">"? Currently, case-based reasoning has been used for structured (tabular) data, static images, and simple sequences such as text."</mark>  [Page 29](zotero://open-pdf/library/items/FYF7GDU4?page=29&annotation=5W6JRMPG) #important, #data-type, #case-based-reasoning, #methods
- <mark class="hltr-green">"Current approaches to prototype learning do not take into account prior knowledge or expert opinions. At times, it may be advantageous to develop prototype-learning algorithms that collaborate with human experts in choosing prototypical cases or prototypical features"</mark>  [Page 30](zotero://open-pdf/library/items/FYF7GDU4?page=30&annotation=L77METCB) #supportingevidence, #case-based-reasoning, #future-research
- <mark class="hltr-green">"n other words, using these constraints, we could constrain our network to have the kind of “Grandmother node” that scientists have been searching for in both real and artificial convolutional neural networks [115]."</mark>  [Page 31](zotero://open-pdf/library/items/FYF7GDU4?page=31&annotation=SBGN6MEG) #Interpretable-machine-learning, #supportingevidence, #disentanglement
- <mark class="hltr-green">"n that sense, vectors in the latent space are “impure” in that they do not naturally represent single concepts [see 58, for a detailed discussion]."</mark>  [Page 32](zotero://open-pdf/library/items/FYF7GDU4?page=32&annotation=CY7BEST3) #critique, #disentanglement

	- we align the axis of the neurons along latent spaces of classes- loading the concepts may take a lot of time if the network has a lot of neurons #critique, #disentanglement
- <mark class="hltr-green">"but this would not mean that the information flow concerning each concept goes only though that concept’s designated path through the network;"</mark>  [Page 33](zotero://open-pdf/library/items/FYF7GDU4?page=33&annotation=79G3A6BT) #critique, #disentanglement
- <mark class="hltr-green">"Perhaps the latter problem could be solved by training with a small random subset of concepts at each iteration; but this has not been tried in current methods at the time of this writing."</mark>  [Page 33](zotero://open-pdf/library/items/FYF7GDU4?page=33&annotation=N5CYJ86G) #future-research, #disentanglement
- <mark class="hltr-green">"How to choose good concepts to learn for disentanglement?"</mark>  [Page 34](zotero://open-pdf/library/items/FYF7GDU4?page=34&annotation=224AU3E5) #important, #disentanglement
- <mark class="hltr-green">"The decision process of current disentangled neural networks contains two parts, x → c mapping the input x to the disentangled representation (concepts) c, and c → y mapping the disentangled representation c to the output y."</mark>  [Page 34](zotero://open-pdf/library/items/FYF7GDU4?page=34&annotation=D6AK8MMK) #Interpretable-machine-learning, #disentanglement

	- there is a gap bc the last output layer is still a blackbox #Interpretable-machine-learning, #disentanglement
- <mark class="hltr-green">"pretability of the latent space and the interpretability of the entire model. Current methods either rely on variable importance methods to explain c → y posthoc [58], or simply make c → y a linear layer [158]."</mark>  [Page 35](zotero://open-pdf/library/items/FYF7GDU4?page=35&annotation=3Q5T8V8A) #Interpretable-machine-learning, #disentanglement

	- use var. importance or posthoc explanations #Interpretable-machine-learning, #disentanglement
- <mark class="hltr-green">"But in the case where we do not know the concepts, or in the case where the concepts are numerous and we do not know how to parameterize them, we cannot use the techniques from Challenge 5. In other words, the concept c in Constraint (5.1) is no longer a concept we predefine, but it must still be an actual concept in the existing universe of concepts"</mark>  [Page 35](zotero://open-pdf/library/items/FYF7GDU4?page=35&annotation=7DW9AIFH) #unsupervised-learning, #challenge, #disentanglement

	- we do not know the classes ahead of time unlike other case. Makes quantitavely evaluating harder if we know nothing about the classes. we may also ignore key iunformaiton if we have human annotators. #unsupervised-learning, #challenge, #disentanglement
- <mark class="hltr-green">"abeled datasets for computer vision have a severe labeling bias: we tend only to label entities in images that are useful for a specific task (e.g., object detection), thus ignoring much of the information found in images."</mark>  [Page 36](zotero://open-pdf/library/items/FYF7GDU4?page=36&annotation=JM3478CN) #unsupervised-learning, #critique, #disentanglement
- <mark class="hltr-green">"Chen et al. [53] propose to create a prototype layer, storing prototypical parts of training images, to do case based reasoning. When classifying birds, the prototypical parts are usually object parts such as heads and wings of birds."</mark>  [Page 38](zotero://open-pdf/library/items/FYF7GDU4?page=38&annotation=EWBW9XK8) #Interpretable-machine-learning, #interesting, #case-based-reasoning, #disentanglement

	- connection between case based reasoning and disentangelemnt to tie back to interpretability of concepts #Interpretable-machine-learning, #interesting, #case-based-reasoning, #disentanglement
- <mark class="hltr-green">"unsupervised disentanglement is desired (but challenging) in two different types of domains: (a) domains in which we do not know what the concepts are (e.g., materials science); (b) domains in which concepts are known but labeling biases exist."</mark>  [Page 39](zotero://open-pdf/library/items/FYF7GDU4?page=39&annotation=4U46X6LW) #important, #unsupervised-learning, #disentanglement
- <mark class="hltr-green">"enerally speaking, there are two primary types of approaches to DR for visualization, commonly referred to as local and global methods. Global methods aim mainly to preserve distances between any pair of points (rather than neighborhoods), while the local methods emphasize preservation of local neighborhoods (that is, which points are nearest neighbors)."</mark>  [Page 41](zotero://open-pdf/library/items/FYF7GDU4?page=41&annotation=FJMNK5LM) #dimension-reduction
- <mark class="hltr-green">"distances from the original space when creating low-dimensional embeddings. But distances between points behave differently in high dimensions than in low dimensions, leading to problems preserving the distances."</mark>  [Page 42](zotero://open-pdf/library/items/FYF7GDU4?page=42&annotation=AGLXZZ9V) #critique, #dimension-reduction

	- also dependent on assumptions about the accuracy of distance metric for data-- not god for neuron weights. not choosing  which hyperparameters are important can lead to loss of global data. #critique, #dimension-reduction
- <mark class="hltr-green">"When their perplexity parameter or the number of nearest neighbors is not chosen carefully, algorithms can fail to preserve the global structure of the mammoth (specifically, the overall placement of the mammoth’s parts), and they create spurious clusters (losing connectivity between parts of the mammoth) and lose details (such as the toes on the feet of the mammoth)"</mark>  [Page 44](zotero://open-pdf/library/items/FYF7GDU4?page=44&annotation=MPT9Q59Q) #critique, #dimension-reduction
- <mark class="hltr-green">"It may be useful to design modern approaches to help users understand how the final two or three dimensions are defined in terms of the high-dimensional features"</mark>  [Page 44](zotero://open-pdf/library/items/FYF7GDU4?page=44&annotation=G259XGR4) #Interpretable-machine-learning, #important, #dimension-reduction

	- not really a god way at the moment to understand PCA and other techniques-- too much complexity for a human. focus on defining realtionships from high dimensional feature to final data with posthoc interpretations. #Interpretable-machine-learning, #important, #dimension-reduction
- <mark class="hltr-green">"Currently, data that might be used for training PINNs are often collected (from experiments or simulations) beforehand (i.e., prior to training of PINNs). This could lead to large uncertainty bands on areas of the input domain where data are scarce, and when the parameters of the PDE need to be learned from these data."</mark>  [Page 47](zotero://open-pdf/library/items/FYF7GDU4?page=47&annotation=7I6AVZCC) #Interpretable-machine-learning, #physics-machine-learning
- <mark class="hltr-green">"neural networks that perform case-based reasoning on disentanglement still yielded models that were equally accurate to their unconstrained values; thus, these interpretable deep neural models are within the Rashomon set"</mark>  [Page 49](zotero://open-pdf/library/items/FYF7GDU4?page=49&annotation=3HHFJ3DR) #Interpretable-machine-learning, #Rashomon-Set, #disentanglement
- <mark class="hltr-green">"think of this as high-dimensional polynomials that are complex enough to fit the data well without overfitting). If a set of simpler functions Fsimpler could serve as approximating set for Fcomplicated (think decision trees of a certain depth approximating the set of polynomials), it means that each complicated function could be well-approximated by a simpler function (and indeed, polynomials can be well-approximated by decision trees). By this logic, the ball of Fcomplicated that is within the Rashomon set must contain at least one function within Fsimpler, which is the simple function we were looking for."</mark>  [Page 49](zotero://open-pdf/library/items/FYF7GDU4?page=49&annotation=MKVHDENS) #important, #Rashomon-Set

	- basically, if we choose model class that doesnt over fit too mich we always have the sipler model we want thats accirate enought (defined by loss threshold) #important, #Rashomon-Set
- <mark class="hltr-green">"Models with various important properties besides interpretability can exist in the Rashomon set, including fairness [67] and monotonicity"</mark>  [Page 50](zotero://open-pdf/library/items/FYF7GDU4?page=50&annotation=HVA24C5Z) #Interpretable-machine-learning, #supportingevidence, #Rashomon-Set
- <mark class="hltr-green">"size of the Rashomon set can be considered as a way of measuring the complexity of a learning problem."</mark>  [Page 50](zotero://open-pdf/library/items/FYF7GDU4?page=50&annotation=9I9EN9SI) #important, #Rashomon-Set
- <mark class="hltr-green">"The Rashomon set can be represented as a subset of this variable importance space"</mark>  [Page 50](zotero://open-pdf/library/items/FYF7GDU4?page=50&annotation=XPIACRUN) #Interpretable-machine-learning, #important, #Rashomon-Set

	- we can set the hypothesis with a latent space of variable importance for models, and see how reliant this variable is across models. #Interpretable-machine-learning, #important, #Rashomon-Set
- <mark class="hltr-green">"Overparametrization or underparametrization can cause volumes in parameter space to be artificially made larger or smaller without a change in the actual space of functions [83]. For instance, if we make a copy of a variable and include it in the datasets, it can change the Rashomon ratio."</mark>  [Page 51](zotero://open-pdf/library/items/FYF7GDU4?page=51&annotation=7NEYXJSF) #important, #Rashomon-Set
- <mark class="hltr-green">"At worst, computation over the Rashomon set requires a brute force calculation over a large discrete hypothesis space. In most cases, the computation should be much easier. Perhaps we could use dynamic programming or branch and bound techniques to reduce the search space so that it encompasses the Rashomon set but not too much more than that?"</mark>  [Page 53](zotero://open-pdf/library/items/FYF7GDU4?page=53&annotation=8VGEYXK9) #important, #Rashomon-Set

	- how to find it #important, #Rashomon-Set
- <mark class="hltr-green">"The success of these techniques most likely will have to depend on whether we can design a good metric for the model class"</mark>  [Page 53](zotero://open-pdf/library/items/FYF7GDU4?page=53&annotation=NRRQHU95) #Rashomon-Set
- <mark class="hltr-green">"Can a similar framework that searches the Rashomon set, instead of the whole hypothesis space, be designed?"</mark>  [Page 54](zotero://open-pdf/library/items/FYF7GDU4?page=54&annotation=4CZ3TUMU) #Rashomon-Set

##  <h1 class="color-blue">Personal Insights</h>
- <mark class="hltr-blue">"Much literature on explainability confounds it with interpretability/comprehensibility"</mark>  [Page 3](zotero://open-pdf/library/items/FYF7GDU4?page=3&annotation=V32LE72Z) #supportingevidence, #Further-exploration-needed

	- What are the most agreed upon definitions here? My interpretation in relation to the most cited sources #supportingevidence, #Further-exploration-needed
- <mark class="hltr-blue">"aim to help readers avoid common but problematic ways of thinking about interpretability in machine learning."</mark>  [Page 3](zotero://open-pdf/library/items/FYF7GDU4?page=3&annotation=VBEEI63H) #Further-exploration-needed, #Interpretability-Principles, #Question

	- Based on the persona, what are common "problematic interpretations" in relation to the domain? #Further-exploration-needed, #Interpretability-Principles, #Question
- <mark class="hltr-blue">"challenge involving additive models"</mark>  [Page 3](zotero://open-pdf/library/items/FYF7GDU4?page=3&annotation=BIK9QFC6) #interpretation, #Interpretable-machine-learning

	- This involves placing constraints on the additivity of models #interpretation, #Interpretable-machine-learning
- <mark class="hltr-blue">"[250]"</mark>  [Page 3](zotero://open-pdf/library/items/FYF7GDU4?page=3&annotation=ZZEDA4L6) #To-read, #Interpretability-Principles

	- expand on principle  1 from initial paper #To-read, #Interpretability-Principles
- <mark class="hltr-blue">"and that each feature is a meaningful predictor of the output on its own."</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=Z95PX9D2) #Further-exploration-needed, #Question

	- Can tabular data have continuous values? what is meant by real, and how do we know it is a meaningful predictor? #Further-exploration-needed, #Question
- <mark class="hltr-blue">"with interactions"</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=XAJLNWSK) #Further-exploration-needed, #Question

	- what interactions in this context? Do the categories potentially have overlap themselves? #Further-exploration-needed, #Question
- <mark class="hltr-blue">"complex interactions (i.e., more than quadratic"</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=AL9QX5JS) #Further-exploration-needed, #Question

	- What are complex interactions? #Further-exploration-needed, #Question
- <mark class="hltr-blue">"small enough that they can be memorized by humans."</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=833SAWMN) #Further-exploration-needed, #Question

	- What kind of data is easy to memorize by people? #Further-exploration-needed, #Question
- <mark class="hltr-blue">"While solutions of (*) would not necessarily be sufficiently interpretable to use in practice, the constraints would generally help us find models that would be interpretable (if we design them well), and we might also be willing to consider slightly suboptimal solutions to find a more useful model."</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=47N64D66) #Further-exploration-needed, #Question, #technical

	- Why is the solution set not fully interperetable? #Further-exploration-needed, #Question, #technical
- <mark class="hltr-blue">"Equation (*) can be generalized to unsupervised learning, where the loss term would simply be replaced by a loss term for the unsupervised problem, whether it is novelty detection, clustering, dimension reduction, or another task."</mark>  [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=UURTFQT8) #Question, #unsupervised-learning, #interesting

	- What is meant by modifiying the loss term? #Question, #unsupervised-learning, #interesting
- <mark class="hltr-blue">"Choices of model form (e.g., the choice to use a decision tree, or a specific neural architecture) are examples of interpretability constraints."</mark>  [Page 5](zotero://open-pdf/library/items/FYF7GDU4?page=5&annotation=RU4MQEF4) #Interpretable-machine-learning, #Further-exploration-needed, #Question, #interpretability-metrics

	- How does choice of the model change the penalty? It is the input to the formula #Interpretable-machine-learning, #Further-exploration-needed, #Question, #interpretability-metrics
- <mark class="hltr-blue">"fully interpretable and partially interpretable models, often preferring the former"</mark>  [Page 5](zotero://open-pdf/library/items/FYF7GDU4?page=5&annotation=4K8UU228) #Further-exploration-needed, #Question

	- The choice of model partially drives the desirability of how interpretable it is. What factors of a model do we consider, and is there a tradeoff in the penalty term? would it be smaller where the desirability for fully interpretable models is high? #Further-exploration-needed, #Question
- <mark class="hltr-blue">"decisions where an explanation would be trivial and the model is 100% reliable"</mark>  [Page 5](zotero://open-pdf/library/items/FYF7GDU4?page=5&annotation=XXIXXXE2) #Question, #confusing

	- Is this based on the classification/output of the model? does the model *need* 100% reliability? #Question, #confusing
- <mark class="hltr-blue">"decisions where humans can verify or modify the decision afterwards"</mark>  [Page 5](zotero://open-pdf/library/items/FYF7GDU4?page=5&annotation=68TFDYXH) #Further-exploration-needed, #disagree

	- Are there frameworks for assessing the reasoning that would benefit from having an interpretability metric?


Otherwise, how could we learn from *why* we modify the decision in the first place, and how we could alter the model later #Further-exploration-needed, #disagree
- <mark class="hltr-blue">"With black boxes, one needs to make a decision about trust with much less information; without knowledge about the reasoning process of the model"</mark>  [Page 6](zotero://open-pdf/library/items/FYF7GDU4?page=6&annotation=I4ERE2YY) #idea, #thought-provoking

	- What frameworks do we use the evaluate a human's reasoning process? #idea, #thought-provoking
- <mark class="hltr-blue">"inflated by including many “obvious” cases"</mark>  [Page 7](zotero://open-pdf/library/items/FYF7GDU4?page=7&annotation=2ZLGQYGM) #question

	- Why are "obvious' cases misleading?
ROC- Distinguishability between classes #question
- <mark class="hltr-blue">"n interpretable robotic surgeon would be worse than its black box counterpart. The question ultimately becomes whether the Rashomon set should permit such an interpretable robotic surgeon–and all scientific evidence so far (including a large-and-growing number of experimental papers on interpretable deep learning) suggests it would."</mark>  [Page 9](zotero://open-pdf/library/items/FYF7GDU4?page=9&annotation=UYI4EFTZ) #question, #blackbox, #Further-exploration-needed

	- What do we mean by "worse"? Are we defining this in terms of accuracy? #question, #blackbox, #Further-exploration-needed
- <mark class="hltr-blue">"Unfortunately, these topics are much too often lumped together within the misleading term “explainable artificial intelligence” or “XAI” despite a chasm separating these two concepts [250]"</mark>  [Page 9](zotero://open-pdf/library/items/FYF7GDU4?page=9&annotation=LWVNQ6QH) #question, #Further-exploration-needed, #definition, #To-read

	- Concretley state the argument between explainability and interpretability. Explainability seems to be the mathematical framework to understand the outcomes of the blackbox, whereas interpretable aims to made predictive models a human can make.


but this is still unclear #question, #Further-exploration-needed, #definition, #To-read
- "<mark class="hltr-blue">"A “saliency” real estate agent would say that the price is determined from the roof and backyard, but doesn’t explain how the roof and backyard were used to determine the price"</mark>" [Page 10](zotero://open-pdf/library/items/FYF7GDU4?page=10&annotation=YFPB3XV8)

	- gives example on what is meant by explaining function approximations 
- <mark class="hltr-blue">"But function approximators are not used in interpretable ML; instead of approximating a known function (a black box ML model), interpretable ML can choose from a potential myriad of approximatelyequally-good models, which, as we noted earlier, is called “the Rashomon set”"</mark>  [Page 11](zotero://open-pdf/library/items/FYF7GDU4?page=11&annotation=LWZI7AK4) #question, #Interpretable-machine-learning, #Explainability

	- difference between model and function in this context #question, #Interpretable-machine-learning, #Explainability
- <mark class="hltr-blue">"linear models, which includes scoring systems (and risk scores)"</mark>  [Page 21](zotero://open-pdf/library/items/FYF7GDU4?page=21&annotation=729DPMNN) #question, #logical-models

	- linear models are logical models? #question, #logical-models
- <mark class="hltr-blue">"The standard form of GAMs is interpretable because the model is constrained to be a linear combination of univariate component functions."</mark>  [Page 22](zotero://open-pdf/library/items/FYF7GDU4?page=22&annotation=88FCURWL) #Interpretable-machine-learning, #important, #Generalized-Additive-Model

	- This is a deterministic function-- different than function approximation #Interpretable-machine-learning, #important, #Generalized-Additive-Model
- <mark class="hltr-blue">"boosted models are not naturally sparse, and issues with bias arise under 1 regularization, as discussed in the scoring systems section."</mark>  [Page 23](zotero://open-pdf/library/items/FYF7GDU4?page=23&annotation=47FY85LE) #question, #Further-exploration-needed, #Generalized-Additive-Model

	- What are proxies? Connects to how regularizaiton issues (stripping away too many small weights) if tree is not sparse can be an issue. #question, #Further-exploration-needed, #Generalized-Additive-Model
- <mark class="hltr-blue">"using a deep neural network that transforms the input space into a feature space where a kNN classifier will perform well (i.e., deep kNN). Papernot and McDaniel [229]"</mark>  [Page 26](zotero://open-pdf/library/items/FYF7GDU4?page=26&annotation=JM7LZQVU) #question

	- what is the relation to latent spaces here? #question
- <mark class="hltr-blue">"prototype-learning algorithms that collaborate with human experts in choosing prototypical cases or prototypical features. For example, in healthcare, it would be beneficial if a prototype-based classifier learns, under the supervision of human doctors"</mark>  [Page 30](zotero://open-pdf/library/items/FYF7GDU4?page=30&annotation=9FGB6R9W) #personal-interest
- <mark class="hltr-blue">"part-whole disentanglement for more complicated patterns in large vision datasets?"</mark>  [Page 40](zotero://open-pdf/library/items/FYF7GDU4?page=40&annotation=6H5PH89S) #important, #idea, #case-based-reasoning, #disentanglement

	- same relation to part-based breakdown as in case- based models with prototypical models. #important, #idea, #case-based-reasoning, #disentanglement
- <mark class="hltr-blue">"This may take the form of explanatory post-hoc visualizations or constrained DR methods."</mark>  [Page 44](zotero://open-pdf/library/items/FYF7GDU4?page=44&annotation=TBHJ8VBI) #Interpretable-machine-learning, #interesting, #idea, #dimension-reduction

	- idea: when us post-hoc or in the loop human decision making for iteratiove model updates better? #Interpretable-machine-learning, #interesting, #idea, #dimension-reduction
- <mark class="hltr-blue">"e size of the Rashomon set differs from all of these quantities in fundamental ways, and it is important in its own right for showing the existence of simpler models."</mark>  [Page 50](zotero://open-pdf/library/items/FYF7GDU4?page=50&annotation=ES8W8MLE) #Further-exploration-needed, #critique, #Rashomon-Set

	- fundemn #Further-exploration-needed, #critique, #Rashomon-Set

##  <h1 class="color-purple">Literary Note To Lookup Later</h>
- <mark class="hltr-purple">"250, 173, 171"</mark>  [Page 2](zotero://open-pdf/library/items/FYF7GDU4?page=2&annotation=NNX8LZMB) #blackbox, #To-read

	- Papers on the mischaracterization issue of black box models #blackbox, #To-read
- <mark class="hltr-purple">"[253]"</mark>  [Page 3](zotero://open-pdf/library/items/FYF7GDU4?page=3&annotation=JR55MZ92) #blackbox, #To-read

	- Black boxes and authority #blackbox, #To-read
- "<mark class="hltr-purple">"understood by humans. These constraints can differ dramatically depending on the domain."</mark>" [Page 4](zotero://open-pdf/library/items/FYF7GDU4?page=4&annotation=AF4UNFQD)
- <mark class="hltr-purple">"157]."</mark>  [Page 5](zotero://open-pdf/library/items/FYF7GDU4?page=5&annotation=WLC7WSIF) #To-read

	- find issues with defining interpertability #To-read
- <mark class="hltr-purple">"COMPAS depends on race other than through age and criminal history [13, 258]"</mark>  [Page 7](zotero://open-pdf/library/items/FYF7GDU4?page=7&annotation=W9TSNVCE) #Interpretable-machine-learning, #To-read, #Question, #bias

	- what does is mean by racial dependence? #Interpretable-machine-learning, #To-read, #Question, #bias
- <mark class="hltr-purple">"hat do not sacrifice accuracy but gain substantial interpretability [333, 53, 158, 58, 12, 216]"</mark>  [Page 8](zotero://open-pdf/library/items/FYF7GDU4?page=8&annotation=D9FN4RNQ) #Interpretable-machine-learning, #blackbox, #To-read

	- papers for intuition about accuracy and interpretability, and how on un-pre-processed datasets, we can get goof accuracy #Interpretable-machine-learning, #blackbox, #To-read
- <mark class="hltr-purple">"The fact that simple models perform well for tabular data could arise from the Rashomon Effect discussed by Leo Breiman [41]."</mark>  [Page 8](zotero://open-pdf/library/items/FYF7GDU4?page=8&annotation=2JHQQIMJ) #Interpretable-machine-learning, #To-read

	- Rashomon Set and intepretability #Interpretable-machine-learning, #To-read
- <mark class="hltr-purple">"Explainability techniques give authority to black box models rather than suggesting the possibility of models that are understandable in the first place [253]"</mark>  [Page 11](zotero://open-pdf/library/items/FYF7GDU4?page=11&annotation=FT5MH46B) #To-read, #Explainability
- <mark class="hltr-purple">"But function approximators are not used in interpretable ML; instead of approximating a known function (a black box ML model), interpretable ML can choose from a potential myriad of approximatelyequally-good models, which, as we noted earlier, is called “the Rashomon set” [41, 97, 269]"</mark>  [Page 11](zotero://open-pdf/library/items/FYF7GDU4?page=11&annotation=7ICAZ5TM) #Interpretable-machine-learning, #important, #Rashomon-Set

	- FA is for explainability(?). We cannot simply construct some equation based on function behavior alone, it must follow constraints from th erashomon set #Interpretable-machine-learning, #important, #Rashomon-Set
- <mark class="hltr-purple">"More recently, Chen et al. [53] extended the work of Li et al. [183] to create a prototypical part network (ProtoPNet) whose prototype layer stores proto Interpretable machine learning grand challenges 29  typical parts of encoded training images. The prototypical parts are patches of convolutional-neural-network-encoded training images, and represent typical features observed for various image classes. Given an input instance, the network compares an encoded input image with each of the learned prototypical parts, and generates a prototype activation map that indicates both the location and the degree of the image patch most similar to that prototypical part. The authors applied the network to the benchmark Caltech-UCSD Birds-200-2011 (CUB-200-2011) dataset [305] for bird recognition, and the ProtoPNet was able to learn prototypical parts of 200 classes of birds, and use these prototypes to classify birds with an accuracy comparable to non-interpretable black-box models."</mark>  [Page 28](zotero://open-pdf/library/items/FYF7GDU4?page=28&annotation=PSEHIAV5) #To-read, #personal-interest
- <mark class="hltr-purple">"Knowledge graphs encode relationships between entities in the world, including common sense knowledge. Thus, being able to incorporate information from a knowledge graph could be very helpful if we can figure out ways to do it effectively."</mark>  [Page 48](zotero://open-pdf/library/items/FYF7GDU4?page=48&annotation=TJAZHZEV) #interesting, #physics-machine-learning, #personal-interest



---
# 🧠 Key Ideas
- 
---
# ⚙️ Project Relations
- 
---
# 📄 Related Literature 
- 
---
# 🏷️ Tags

# Unique tag Groups 

#Further-exploration-needed, #definition
#actionitem, #definition
#actionitem, #important, #definition
#blackbox, #supportingevidence, #Further-exploration-needed
#Interpretable-machine-learning, #Further-exploration-needed, #definition
#supportingevidence
#actionitem, #important, #blackbox, #definition
#blackbox, #supportingevidence
#Interpretable-machine-learning, #actionitem, #definition
#blackbox, #To-read
#supportingevidence, #Further-exploration-needed
#Further-exploration-needed, #Interpretability-Principles, #Question
#Interpretable-machine-learning, #important, #Interpretability-Principles
#interpretation, #Interpretable-machine-learning
#To-read, #Interpretability-Principles
#important, #Interpretability-Principles
#definition
#Further-exploration-needed, #Question
#Interpretable-machine-learning, #formula
#example
#Further-exploration-needed, #Question, #technical
#Question, #unsupervised-learning, #interesting
#Interpretable-machine-learning, #counterargument
#Interpretable-machine-learning, #important, #Further-exploration-needed, #definition
#To-read
#Interpretable-machine-learning, #performance-metrics
#Interpretable-machine-learning, #Further-exploration-needed, #Question, #interpretability-metrics
#Question, #confusing
#Further-exploration-needed, #disagree
#idea, #thought-provoking
#Interpretable-machine-learning, #critique
#Interpretable-machine-learning, #important
#Interpretable-machine-learning, #To-read, #Question, #bias
#question
#Interpretable-machine-learning, #blackbox, #To-read
#blackbox, #critique
#Interpretable-machine-learning, #To-read
#question, #blackbox, #Further-exploration-needed
#Interpretability-Principles
#Further-exploration-needed, #Interpretability-Principles
#question, #Further-exploration-needed, #definition, #To-read
#question, #Interpretable-machine-learning, #critique, #Explainability
#critique, #Explainability
#To-read, #Explainability
#question, #Interpretable-machine-learning, #Explainability
#Interpretable-machine-learning, #important, #Rashomon-Set
#Interpretable-machine-learning, #supportingevidence, #data-type, #logical-model
#logical-model
#formula, #sparsity
#important, #logical-model
#definition, #logical-model
#critique, #logical-model
#logical-model, #solution
#logical-model, #challenge
#Rashomon-Set, #logical-model
#Rashomon-Set, #logical
#question, #logical-models
#formula
#Interpretable-machine-learning, #important, #Generalized-Additive-Model
#Generalized-Additive-Model, #equation
#question, #Further-exploration-needed, #Generalized-Additive-Model
#important, #Generalized-Additive-Model
#data-type, #Generalized-Additive-Model
#definition, #case-based-reasoning
#supportingevidence, #case-based-reasoning
#case-based-reasoning, #methods
#critique, #case-based-reasoning
#example, #case-based-reasoning
#To-read, #personal-interest
#important, #data-type, #case-based-reasoning, #methods
#supportingevidence, #case-based-reasoning, #future-research
#personal-interest
#definition, #disentanglement
#Interpretable-machine-learning, #supportingevidence, #disentanglement
#critique, #disentanglement
#future-research, #disentanglement
#important, #disentanglement
#Interpretable-machine-learning, #disentanglement
#unsupervised-learning, #challenge, #disentanglement
#unsupervised-learning, #critique, #disentanglement
#Interpretable-machine-learning, #interesting, #case-based-reasoning, #disentanglement
#important, #unsupervised-learning, #disentanglement
#important, #idea, #case-based-reasoning, #disentanglement
#dimension-reduction
#critique, #dimension-reduction
#Interpretable-machine-learning, #important, #dimension-reduction
#Interpretable-machine-learning, #interesting, #idea, #dimension-reduction
#definition, #physics-machine-learning
#physics-machine-learning, #method
#Interpretable-machine-learning, #physics-machine-learning
#interesting, #physics-machine-learning, #personal-interest
#definition, #Rashomon-Set
#Interpretable-machine-learning, #Rashomon-Set, #disentanglement
#formula, #Rashomon-Set
#important, #Rashomon-Set
#Interpretable-machine-learning, #supportingevidence, #Rashomon-Set
#Further-exploration-needed, #critique, #Rashomon-Set
#Rashomon-Set


# 🏷️ Tags Groups within Current Paper
# #Further-exploration-needed, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #definition")
WHERE file.path = this.file.path
```


# #actionitem, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#actionitem, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#actionitem, #definition")
WHERE file.path = this.file.path
```


# #actionitem, #important, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#actionitem, #important, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#actionitem, #important, #definition")
WHERE file.path = this.file.path
```


# #blackbox, #supportingevidence, #Further-exploration-needed

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#blackbox, #supportingevidence, #Further-exploration-needed", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#blackbox, #supportingevidence, #Further-exploration-needed")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #Further-exploration-needed, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #Further-exploration-needed, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #Further-exploration-needed, #definition")
WHERE file.path = this.file.path
```


# #supportingevidence

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#supportingevidence", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#supportingevidence")
WHERE file.path = this.file.path
```


# #actionitem, #important, #blackbox, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#actionitem, #important, #blackbox, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#actionitem, #important, #blackbox, #definition")
WHERE file.path = this.file.path
```


# #blackbox, #supportingevidence

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#blackbox, #supportingevidence", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#blackbox, #supportingevidence")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #actionitem, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #actionitem, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #actionitem, #definition")
WHERE file.path = this.file.path
```


# #blackbox, #To-read

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#blackbox, #To-read", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#blackbox, #To-read")
WHERE file.path = this.file.path
```


# #supportingevidence, #Further-exploration-needed

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#supportingevidence, #Further-exploration-needed", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#supportingevidence, #Further-exploration-needed")
WHERE file.path = this.file.path
```


# #Further-exploration-needed, #Interpretability-Principles, #Question

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #Interpretability-Principles, #Question", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #Interpretability-Principles, #Question")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #important, #Interpretability-Principles

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important, #Interpretability-Principles", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important, #Interpretability-Principles")
WHERE file.path = this.file.path
```


# #interpretation, #Interpretable-machine-learning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#interpretation, #Interpretable-machine-learning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#interpretation, #Interpretable-machine-learning")
WHERE file.path = this.file.path
```


# #To-read, #Interpretability-Principles

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#To-read, #Interpretability-Principles", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#To-read, #Interpretability-Principles")
WHERE file.path = this.file.path
```


# #important, #Interpretability-Principles

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #Interpretability-Principles", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #Interpretability-Principles")
WHERE file.path = this.file.path
```


# #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition")
WHERE file.path = this.file.path
```


# #Further-exploration-needed, #Question

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #Question", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #Question")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #formula

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #formula", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #formula")
WHERE file.path = this.file.path
```


# #example

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#example", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#example")
WHERE file.path = this.file.path
```


# #Further-exploration-needed, #Question, #technical

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #Question, #technical", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #Question, #technical")
WHERE file.path = this.file.path
```


# #Question, #unsupervised-learning, #interesting

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Question, #unsupervised-learning, #interesting", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Question, #unsupervised-learning, #interesting")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #counterargument

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #counterargument", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #counterargument")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #important, #Further-exploration-needed, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important, #Further-exploration-needed, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important, #Further-exploration-needed, #definition")
WHERE file.path = this.file.path
```


# #To-read

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#To-read", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#To-read")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #performance-metrics

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #performance-metrics", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #performance-metrics")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #Further-exploration-needed, #Question, #interpretability-metrics

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #Further-exploration-needed, #Question, #interpretability-metrics", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #Further-exploration-needed, #Question, #interpretability-metrics")
WHERE file.path = this.file.path
```


# #Question, #confusing

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Question, #confusing", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Question, #confusing")
WHERE file.path = this.file.path
```


# #Further-exploration-needed, #disagree

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #disagree", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #disagree")
WHERE file.path = this.file.path
```


# #idea, #thought-provoking

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#idea, #thought-provoking", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#idea, #thought-provoking")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #critique

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #critique", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #critique")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #important

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #To-read, #Question, #bias

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #To-read, #Question, #bias", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #To-read, #Question, #bias")
WHERE file.path = this.file.path
```


# #question

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #blackbox, #To-read

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #blackbox, #To-read", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #blackbox, #To-read")
WHERE file.path = this.file.path
```


# #blackbox, #critique

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#blackbox, #critique", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#blackbox, #critique")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #To-read

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #To-read", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #To-read")
WHERE file.path = this.file.path
```


# #question, #blackbox, #Further-exploration-needed

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #blackbox, #Further-exploration-needed", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #blackbox, #Further-exploration-needed")
WHERE file.path = this.file.path
```


# #Interpretability-Principles

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretability-Principles", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretability-Principles")
WHERE file.path = this.file.path
```


# #Further-exploration-needed, #Interpretability-Principles

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #Interpretability-Principles", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #Interpretability-Principles")
WHERE file.path = this.file.path
```


# #question, #Further-exploration-needed, #definition, #To-read

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #Further-exploration-needed, #definition, #To-read", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #Further-exploration-needed, #definition, #To-read")
WHERE file.path = this.file.path
```


# #question, #Interpretable-machine-learning, #critique, #Explainability

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #Interpretable-machine-learning, #critique, #Explainability", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #Interpretable-machine-learning, #critique, #Explainability")
WHERE file.path = this.file.path
```


# #critique, #Explainability

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#critique, #Explainability", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#critique, #Explainability")
WHERE file.path = this.file.path
```


# #To-read, #Explainability

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#To-read, #Explainability", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#To-read, #Explainability")
WHERE file.path = this.file.path
```


# #question, #Interpretable-machine-learning, #Explainability

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #Interpretable-machine-learning, #Explainability", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #Interpretable-machine-learning, #Explainability")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #important, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important, #Rashomon-Set")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #supportingevidence, #data-type, #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #supportingevidence, #data-type, #logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #supportingevidence, #data-type, #logical-model")
WHERE file.path = this.file.path
```


# #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#logical-model")
WHERE file.path = this.file.path
```


# #formula, #sparsity

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#formula, #sparsity", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#formula, #sparsity")
WHERE file.path = this.file.path
```


# #important, #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #logical-model")
WHERE file.path = this.file.path
```


# #definition, #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition, #logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition, #logical-model")
WHERE file.path = this.file.path
```


# #critique, #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#critique, #logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#critique, #logical-model")
WHERE file.path = this.file.path
```


# #logical-model, #solution

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#logical-model, #solution", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#logical-model, #solution")
WHERE file.path = this.file.path
```


# #logical-model, #challenge

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#logical-model, #challenge", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#logical-model, #challenge")
WHERE file.path = this.file.path
```


# #Rashomon-Set, #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Rashomon-Set, #logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Rashomon-Set, #logical-model")
WHERE file.path = this.file.path
```


# #Rashomon-Set, #logical

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Rashomon-Set, #logical", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Rashomon-Set, #logical")
WHERE file.path = this.file.path
```


# #question, #logical-models

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #logical-models", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #logical-models")
WHERE file.path = this.file.path
```


# #formula

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#formula", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#formula")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #important, #Generalized-Additive-Model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important, #Generalized-Additive-Model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important, #Generalized-Additive-Model")
WHERE file.path = this.file.path
```


# #Generalized-Additive-Model, #equation

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Generalized-Additive-Model, #equation", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Generalized-Additive-Model, #equation")
WHERE file.path = this.file.path
```


# #question, #Further-exploration-needed, #Generalized-Additive-Model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #Further-exploration-needed, #Generalized-Additive-Model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #Further-exploration-needed, #Generalized-Additive-Model")
WHERE file.path = this.file.path
```


# #important, #Generalized-Additive-Model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #Generalized-Additive-Model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #Generalized-Additive-Model")
WHERE file.path = this.file.path
```


# #data-type, #Generalized-Additive-Model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#data-type, #Generalized-Additive-Model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#data-type, #Generalized-Additive-Model")
WHERE file.path = this.file.path
```


# #definition, #case-based-reasoning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition, #case-based-reasoning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition, #case-based-reasoning")
WHERE file.path = this.file.path
```


# #supportingevidence, #case-based-reasoning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#supportingevidence, #case-based-reasoning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#supportingevidence, #case-based-reasoning")
WHERE file.path = this.file.path
```


# #case-based-reasoning, #methods

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#case-based-reasoning, #methods", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#case-based-reasoning, #methods")
WHERE file.path = this.file.path
```


# #critique, #case-based-reasoning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#critique, #case-based-reasoning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#critique, #case-based-reasoning")
WHERE file.path = this.file.path
```


# #example, #case-based-reasoning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#example, #case-based-reasoning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#example, #case-based-reasoning")
WHERE file.path = this.file.path
```


# #To-read, #personal-interest

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#To-read, #personal-interest", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#To-read, #personal-interest")
WHERE file.path = this.file.path
```


# #important, #data-type, #case-based-reasoning, #methods

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #data-type, #case-based-reasoning, #methods", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #data-type, #case-based-reasoning, #methods")
WHERE file.path = this.file.path
```


# #supportingevidence, #case-based-reasoning, #future-research

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#supportingevidence, #case-based-reasoning, #future-research", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#supportingevidence, #case-based-reasoning, #future-research")
WHERE file.path = this.file.path
```


# #personal-interest

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#personal-interest", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#personal-interest")
WHERE file.path = this.file.path
```


# #definition, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition, #disentanglement")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #supportingevidence, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #supportingevidence, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #supportingevidence, #disentanglement")
WHERE file.path = this.file.path
```


# #critique, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#critique, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#critique, #disentanglement")
WHERE file.path = this.file.path
```


# #future-research, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#future-research, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#future-research, #disentanglement")
WHERE file.path = this.file.path
```


# #important, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #disentanglement")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #disentanglement")
WHERE file.path = this.file.path
```


# #unsupervised-learning, #challenge, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#unsupervised-learning, #challenge, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#unsupervised-learning, #challenge, #disentanglement")
WHERE file.path = this.file.path
```


# #unsupervised-learning, #critique, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#unsupervised-learning, #critique, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#unsupervised-learning, #critique, #disentanglement")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #interesting, #case-based-reasoning, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #interesting, #case-based-reasoning, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #interesting, #case-based-reasoning, #disentanglement")
WHERE file.path = this.file.path
```


# #important, #unsupervised-learning, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #unsupervised-learning, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #unsupervised-learning, #disentanglement")
WHERE file.path = this.file.path
```


# #important, #idea, #case-based-reasoning, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #idea, #case-based-reasoning, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #idea, #case-based-reasoning, #disentanglement")
WHERE file.path = this.file.path
```


# #dimension-reduction

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#dimension-reduction", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#dimension-reduction")
WHERE file.path = this.file.path
```


# #critique, #dimension-reduction

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#critique, #dimension-reduction", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#critique, #dimension-reduction")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #important, #dimension-reduction

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important, #dimension-reduction", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important, #dimension-reduction")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #interesting, #idea, #dimension-reduction

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #interesting, #idea, #dimension-reduction", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #interesting, #idea, #dimension-reduction")
WHERE file.path = this.file.path
```


# #definition, #physics-machine-learning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition, #physics-machine-learning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition, #physics-machine-learning")
WHERE file.path = this.file.path
```


# #physics-machine-learning, #method

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#physics-machine-learning, #method", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#physics-machine-learning, #method")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #physics-machine-learning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #physics-machine-learning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #physics-machine-learning")
WHERE file.path = this.file.path
```


# #interesting, #physics-machine-learning, #personal-interest

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#interesting, #physics-machine-learning, #personal-interest", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#interesting, #physics-machine-learning, #personal-interest")
WHERE file.path = this.file.path
```


# #definition, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition, #Rashomon-Set")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #Rashomon-Set, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #Rashomon-Set, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #Rashomon-Set, #disentanglement")
WHERE file.path = this.file.path
```


# #formula, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#formula, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#formula, #Rashomon-Set")
WHERE file.path = this.file.path
```


# #important, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #Rashomon-Set")
WHERE file.path = this.file.path
```


# #Interpretable-machine-learning, #supportingevidence, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #supportingevidence, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #supportingevidence, #Rashomon-Set")
WHERE file.path = this.file.path
```


# #Further-exploration-needed, #critique, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #critique, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #critique, #Rashomon-Set")
WHERE file.path = this.file.path
```


# #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Rashomon-Set")
WHERE file.path = this.file.path
```



---

# 🏷️ Tags Groups within All Papers
# #Further-exploration-needed, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #definition")
```


# #actionitem, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#actionitem, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#actionitem, #definition")
```


# #actionitem, #important, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#actionitem, #important, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#actionitem, #important, #definition")
```


# #blackbox, #supportingevidence, #Further-exploration-needed

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#blackbox, #supportingevidence, #Further-exploration-needed", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#blackbox, #supportingevidence, #Further-exploration-needed")
```


# #Interpretable-machine-learning, #Further-exploration-needed, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #Further-exploration-needed, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #Further-exploration-needed, #definition")
```


# #supportingevidence

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#supportingevidence", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#supportingevidence")
```


# #actionitem, #important, #blackbox, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#actionitem, #important, #blackbox, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#actionitem, #important, #blackbox, #definition")
```


# #blackbox, #supportingevidence

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#blackbox, #supportingevidence", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#blackbox, #supportingevidence")
```


# #Interpretable-machine-learning, #actionitem, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #actionitem, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #actionitem, #definition")
```


# #blackbox, #To-read

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#blackbox, #To-read", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#blackbox, #To-read")
```


# #supportingevidence, #Further-exploration-needed

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#supportingevidence, #Further-exploration-needed", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#supportingevidence, #Further-exploration-needed")
```


# #Further-exploration-needed, #Interpretability-Principles, #Question

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #Interpretability-Principles, #Question", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #Interpretability-Principles, #Question")
```


# #Interpretable-machine-learning, #important, #Interpretability-Principles

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important, #Interpretability-Principles", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important, #Interpretability-Principles")
```


# #interpretation, #Interpretable-machine-learning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#interpretation, #Interpretable-machine-learning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#interpretation, #Interpretable-machine-learning")
```


# #To-read, #Interpretability-Principles

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#To-read, #Interpretability-Principles", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#To-read, #Interpretability-Principles")
```


# #important, #Interpretability-Principles

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #Interpretability-Principles", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #Interpretability-Principles")
```


# #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition")
```


# #Further-exploration-needed, #Question

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #Question", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #Question")
```


# #Interpretable-machine-learning, #formula

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #formula", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #formula")
```


# #example

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#example", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#example")
```


# #Further-exploration-needed, #Question, #technical

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #Question, #technical", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #Question, #technical")
```


# #Question, #unsupervised-learning, #interesting

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Question, #unsupervised-learning, #interesting", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Question, #unsupervised-learning, #interesting")
```


# #Interpretable-machine-learning, #counterargument

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #counterargument", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #counterargument")
```


# #Interpretable-machine-learning, #important, #Further-exploration-needed, #definition

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important, #Further-exploration-needed, #definition", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important, #Further-exploration-needed, #definition")
```


# #To-read

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#To-read", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#To-read")
```


# #Interpretable-machine-learning, #performance-metrics

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #performance-metrics", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #performance-metrics")
```


# #Interpretable-machine-learning, #Further-exploration-needed, #Question, #interpretability-metrics

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #Further-exploration-needed, #Question, #interpretability-metrics", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #Further-exploration-needed, #Question, #interpretability-metrics")
```


# #Question, #confusing

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Question, #confusing", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Question, #confusing")
```


# #Further-exploration-needed, #disagree

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #disagree", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #disagree")
```


# #idea, #thought-provoking

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#idea, #thought-provoking", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#idea, #thought-provoking")
```


# #Interpretable-machine-learning, #critique

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #critique", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #critique")
```


# #Interpretable-machine-learning, #important

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important")
```


# #Interpretable-machine-learning, #To-read, #Question, #bias

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #To-read, #Question, #bias", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #To-read, #Question, #bias")
```


# #question

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question")
```


# #Interpretable-machine-learning, #blackbox, #To-read

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #blackbox, #To-read", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #blackbox, #To-read")
```


# #blackbox, #critique

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#blackbox, #critique", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#blackbox, #critique")
```


# #Interpretable-machine-learning, #To-read

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #To-read", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #To-read")
```


# #question, #blackbox, #Further-exploration-needed

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #blackbox, #Further-exploration-needed", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #blackbox, #Further-exploration-needed")
```


# #Interpretability-Principles

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretability-Principles", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretability-Principles")
```


# #Further-exploration-needed, #Interpretability-Principles

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #Interpretability-Principles", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #Interpretability-Principles")
```


# #question, #Further-exploration-needed, #definition, #To-read

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #Further-exploration-needed, #definition, #To-read", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #Further-exploration-needed, #definition, #To-read")
```


# #question, #Interpretable-machine-learning, #critique, #Explainability

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #Interpretable-machine-learning, #critique, #Explainability", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #Interpretable-machine-learning, #critique, #Explainability")
```


# #critique, #Explainability

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#critique, #Explainability", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#critique, #Explainability")
```


# #To-read, #Explainability

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#To-read, #Explainability", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#To-read, #Explainability")
```


# #question, #Interpretable-machine-learning, #Explainability

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #Interpretable-machine-learning, #Explainability", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #Interpretable-machine-learning, #Explainability")
```


# #Interpretable-machine-learning, #important, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important, #Rashomon-Set")
```


# #Interpretable-machine-learning, #supportingevidence, #data-type, #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #supportingevidence, #data-type, #logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #supportingevidence, #data-type, #logical-model")
```


# #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#logical-model")
```


# #formula, #sparsity

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#formula, #sparsity", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#formula, #sparsity")
```


# #important, #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #logical-model")
```


# #definition, #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition, #logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition, #logical-model")
```


# #critique, #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#critique, #logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#critique, #logical-model")
```


# #logical-model, #solution

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#logical-model, #solution", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#logical-model, #solution")
```


# #logical-model, #challenge

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#logical-model, #challenge", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#logical-model, #challenge")
```


# #Rashomon-Set, #logical-model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Rashomon-Set, #logical-model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Rashomon-Set, #logical-model")
```


# #Rashomon-Set, #logical

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Rashomon-Set, #logical", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Rashomon-Set, #logical")
```


# #question, #logical-models

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #logical-models", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #logical-models")
```


# #formula

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#formula", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#formula")
```


# #Interpretable-machine-learning, #important, #Generalized-Additive-Model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important, #Generalized-Additive-Model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important, #Generalized-Additive-Model")
```


# #Generalized-Additive-Model, #equation

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Generalized-Additive-Model, #equation", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Generalized-Additive-Model, #equation")
```


# #question, #Further-exploration-needed, #Generalized-Additive-Model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#question, #Further-exploration-needed, #Generalized-Additive-Model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#question, #Further-exploration-needed, #Generalized-Additive-Model")
```


# #important, #Generalized-Additive-Model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #Generalized-Additive-Model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #Generalized-Additive-Model")
```


# #data-type, #Generalized-Additive-Model

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#data-type, #Generalized-Additive-Model", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#data-type, #Generalized-Additive-Model")
```


# #definition, #case-based-reasoning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition, #case-based-reasoning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition, #case-based-reasoning")
```


# #supportingevidence, #case-based-reasoning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#supportingevidence, #case-based-reasoning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#supportingevidence, #case-based-reasoning")
```


# #case-based-reasoning, #methods

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#case-based-reasoning, #methods", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#case-based-reasoning, #methods")
```


# #critique, #case-based-reasoning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#critique, #case-based-reasoning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#critique, #case-based-reasoning")
```


# #example, #case-based-reasoning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#example, #case-based-reasoning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#example, #case-based-reasoning")
```


# #To-read, #personal-interest

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#To-read, #personal-interest", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#To-read, #personal-interest")
```


# #important, #data-type, #case-based-reasoning, #methods

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #data-type, #case-based-reasoning, #methods", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #data-type, #case-based-reasoning, #methods")
```


# #supportingevidence, #case-based-reasoning, #future-research

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#supportingevidence, #case-based-reasoning, #future-research", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#supportingevidence, #case-based-reasoning, #future-research")
```


# #personal-interest

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#personal-interest", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#personal-interest")
```


# #definition, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition, #disentanglement")
```


# #Interpretable-machine-learning, #supportingevidence, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #supportingevidence, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #supportingevidence, #disentanglement")
```


# #critique, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#critique, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#critique, #disentanglement")
```


# #future-research, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#future-research, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#future-research, #disentanglement")
```


# #important, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #disentanglement")
```


# #Interpretable-machine-learning, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #disentanglement")
```


# #unsupervised-learning, #challenge, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#unsupervised-learning, #challenge, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#unsupervised-learning, #challenge, #disentanglement")
```


# #unsupervised-learning, #critique, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#unsupervised-learning, #critique, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#unsupervised-learning, #critique, #disentanglement")
```


# #Interpretable-machine-learning, #interesting, #case-based-reasoning, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #interesting, #case-based-reasoning, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #interesting, #case-based-reasoning, #disentanglement")
```


# #important, #unsupervised-learning, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #unsupervised-learning, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #unsupervised-learning, #disentanglement")
```


# #important, #idea, #case-based-reasoning, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #idea, #case-based-reasoning, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #idea, #case-based-reasoning, #disentanglement")
```


# #dimension-reduction

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#dimension-reduction", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#dimension-reduction")
```


# #critique, #dimension-reduction

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#critique, #dimension-reduction", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#critique, #dimension-reduction")
```


# #Interpretable-machine-learning, #important, #dimension-reduction

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #important, #dimension-reduction", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #important, #dimension-reduction")
```


# #Interpretable-machine-learning, #interesting, #idea, #dimension-reduction

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #interesting, #idea, #dimension-reduction", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #interesting, #idea, #dimension-reduction")
```


# #definition, #physics-machine-learning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition, #physics-machine-learning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition, #physics-machine-learning")
```


# #physics-machine-learning, #method

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#physics-machine-learning, #method", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#physics-machine-learning, #method")
```


# #Interpretable-machine-learning, #physics-machine-learning

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #physics-machine-learning", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #physics-machine-learning")
```


# #interesting, #physics-machine-learning, #personal-interest

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#interesting, #physics-machine-learning, #personal-interest", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#interesting, #physics-machine-learning, #personal-interest")
```


# #definition, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#definition, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#definition, #Rashomon-Set")
```


# #Interpretable-machine-learning, #Rashomon-Set, #disentanglement

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #Rashomon-Set, #disentanglement", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #Rashomon-Set, #disentanglement")
```


# #formula, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#formula, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#formula, #Rashomon-Set")
```


# #important, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#important, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#important, #Rashomon-Set")
```


# #Interpretable-machine-learning, #supportingevidence, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Interpretable-machine-learning, #supportingevidence, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Interpretable-machine-learning, #supportingevidence, #Rashomon-Set")
```


# #Further-exploration-needed, #critique, #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Further-exploration-needed, #critique, #Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Further-exploration-needed, #critique, #Rashomon-Set")
```


# #Rashomon-Set

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "#Rashomon-Set", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "#Rashomon-Set")
```




