---
tags:
  - 📥️/📜️/🟥️
publish: false
aliases:
  - Interpretable machine learning Fundamental principles and 10 grand challenges
  - rudinInterpretableMachineLearning2022
---
annotated summary: [[rudinInterpretableMachineLearning2022]]

> [!link]
> zotero_link:: [Rudin et al. - 2022 - Interpretable machine learning Fundamental principles and 10 grand challenges.pdf](zotero://select/library/items/SEK5XBGS)

> [!cite]
> citekey:: rudinInterpretableMachineLearning2022

> [!abstract]
> abstract:: Interpretability in machine learning (ML) is crucial for high stakes decisions and troubleshooting. In this work, we provide fundamental principles for interpretable ML, and dispel common misunderstandings that dilute the importance of this crucial topic. We also identify 10 technical challenge areas in interpretable machine learning and provide history and background on each problem. Some of these problems are classically important, and some are recent problems that have arisen in the last few years. These problems are: (1) Optimizing sparse logical models such as decision trees; (2) Optimization of scoring systems; (3) Placing constraints into generalized additive models to encourage sparsity and better interpretability; (4) Modern case-based reasoning, including neural networks and matching for causal inference; (5) Complete supervised disentanglement of neural networks; (6) Complete or even partial unsupervised disentanglement of neural networks; (7) Dimensionality reduction for data visualization; (8) Machine learning models that can incorporate physics and other generative or causal constraints; (9) Characterization of the “Rashomon set” of good models; and (10) Interpretable reinforcement learning. This survey is suitable as a starting point for statisticians and computer scientists interested in working in interpretable machine learning.

> [!keywords]
> keywords:: 62-02, 68T01, explainable machine learning, Interpretable machine learning

> [!authors]
> authors:: Cynthia Rudin, Chaofan Chen, Zhi Chen, Haiyang Huang, Lesia Semenova, Chudi Zhong

> [!meta]
> url:: https://projecteuclid.org/journals/statistics-surveys/volume-16/issue-none/Interpretable-machine-learning-Fundamental-principles-and-10-grand-challenges/10.1214/21-SS133.full
> doi:: 

> [!related]

```dataview
TABLE created, updated as modified, tags, type
FROM ""
WHERE related != null
AND contains(related, "rudinInterpretableMachineLearning2022")
```

> [!hypothesis]
> hypothesis:: 

> [!methodology] 
> methodology:: 

> [!result] Result(s) 
> results::

> [!summary] Summary of Key Points
> summary:: 

## Notes

| <mark class="hltr-grey">Highlight Color</mark> | Meaning                       |
| ---------------------------------------------- | ----------------------------- |
| <mark class="hltr-red">Red</mark>              | Disagree with Author          |
| <mark class="hltr-orange">Orange</mark>        | Important Point By Author     |
| <mark class="hltr-yellow">Yellow</mark>        | Interesting Point             |
| <mark class="hltr-green">Green</mark>          | Important To Me               |
| <mark class="hltr-blue">Blue</mark>            | Notes After Initial Iteration |
| <mark class="hltr-purple">Purple</mark>        | Literary Note To Lookup Later |

- <mark class="hltr-red">"case-based reasoning”</mark> [Page ](zotero://open-pdf/library/items/SEK5XBGS?page=&annotation=4X946TPU) 
	- define and find examples 
- <mark class="hltr-red">"disentanglement of neural networks”</mark> [Page ](zotero://open-pdf/library/items/SEK5XBGS?page=&annotation=DKFSZ6PY) 
	- define disentanglement 
- <mark class="hltr-red">"generative or causal constraints”</mark> [Page ](zotero://open-pdf/library/items/SEK5XBGS?page=&annotation=REY5CCYY) 
	- find examples and define 
- <mark class="hltr-red">"“Rashomon set””</mark> [Page ](zotero://open-pdf/library/items/SEK5XBGS?page=&annotation=2SKICXV2) 
	- Define 
- <mark class="hltr-green">"Black box predictive models, which by definition are inscrutable, have led to serious societal problems that deeply affect health, freedom, racial bias, and safety.”</mark> [Page 2](zotero://open-pdf/library/items/SEK5XBGS?page=2&annotation=L5KACVJW) 
- <mark class="hltr-red">"Interpretable predictive models, which are constrained so that their reasoning processes are more understandable to humans”</mark> [Page 2](zotero://open-pdf/library/items/SEK5XBGS?page=2&annotation=9TV29SCN) 
	- high level defintion of interpretability the paper uses as basis for defintion. Could refine further 
- <mark class="hltr-green">"black box machine learning model is a formula that is either too complicated for any human to understand, or proprietary”</mark> [Page 2](zotero://open-pdf/library/items/SEK5XBGS?page=2&annotation=I8SRNF7V) 
- <mark class="hltr-red">"“Clever Hans” phenomenon”</mark> [Page 2](zotero://open-pdf/library/items/SEK5XBGS?page=2&annotation=Y7Z5ZL8S) 
	- Need to define in relation to impact of using black box models in practice 
- <mark class="hltr-green">"individuals may have been subjected to years of extra prison time due to typographical errors”</mark> [Page 2](zotero://open-pdf/library/items/SEK5XBGS?page=2&annotation=PTIGNX78) 
- <mark class="hltr-green">"poorly-designed proprietary models for air quality have had serious consequences for public safety during wildfires”</mark> [Page 2](zotero://open-pdf/library/items/SEK5XBGS?page=2&annotation=J5WZFKVB) 
- <mark class="hltr-red">"underlying distribution of data changes (called domain shift”</mark> [Page 2](zotero://open-pdf/library/items/SEK5XBGS?page=2&annotation=MVGFEPEC) 
	- define domain shift, and whether thee are generalize frameworks for how this arises in 2-3 key domains were interperetability has a huge effect. 
- <mark class="hltr-green">"Explaining black boxes, rather than replacing them with interpretable models, can make the problem worse by providing misleading or false characterizations”</mark> [Page 2](zotero://open-pdf/library/items/SEK5XBGS?page=2&annotation=4ZF8ZIK3) 
- <mark class="hltr-purple">"250, 173, 171”</mark> [Page 2](zotero://open-pdf/library/items/SEK5XBGS?page=2&annotation=NNX8LZMB) 
	- Papers on the mischaracterization issue of black box models 
- <mark class="hltr-purple">"[253]”</mark> [Page 3](zotero://open-pdf/library/items/SEK5XBGS?page=3&annotation=JR55MZ92) 
	- Black boxes and authority 
- <mark class="hltr-blue">"Much literature on explainability confounds it with interpretability/comprehensibility”</mark> [Page 3](zotero://open-pdf/library/items/SEK5XBGS?page=3&annotation=V32LE72Z) 
	- What are the most agreed upon definitions here? My interpretation in relation to the most cited sources 
- <mark class="hltr-green">"one would explain a black box without consideration of whether there is an interpretable model of the same accuracy”</mark> [Page 3](zotero://open-pdf/library/items/SEK5XBGS?page=3&annotation=4LYI9PTB) 
	- In what areas is this becoming an increasing need?


What are some common themes among black box papers that lead to poor explainability ? 
- <mark class="hltr-blue">"aim to help readers avoid common but problematic ways of thinking about interpretability in machine learning.”</mark> [Page 3](zotero://open-pdf/library/items/SEK5XBGS?page=3&annotation=VBEEI63H) 
	- Based on the persona, what are common "problematic interpretations" in relation to the domain? 
- <mark class="hltr-magenta">"how to build sparse models for tabular data, including decision trees”</mark> [Page 3](zotero://open-pdf/library/items/SEK5XBGS?page=3&annotation=L6G8KV4Q) 
- <mark class="hltr-blue">"challenge involving additive models”</mark> [Page 3](zotero://open-pdf/library/items/SEK5XBGS?page=3&annotation=BIK9QFC6) 
	- This involves placing constraints on the additivity of models 
- <mark class="hltr-blue">"[250]”</mark> [Page 3](zotero://open-pdf/library/items/SEK5XBGS?page=3&annotation=ZZEDA4L6) 
	- expand on principle  1 from initial paper 
- <mark class="hltr-magenta">"Principle 1 An interpretable machine learning model obeys a domain-specific set of constraints to allow it (or its predictions, or the data)”</mark> [Page 3](zotero://open-pdf/library/items/SEK5XBGS?page=3&annotation=Z67W59UA) 
- <mark class="hltr-red">"Clean” means that the data do not have too much noise or systematic bias”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=SHSC968Q) 
- <mark class="hltr-red">"Tabular” means that the features are categorical or real,”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=5UKBRRZY) 
- <mark class="hltr-blue">"and that each feature is a meaningful predictor of the output on its own.”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=Z95PX9D2) 
	- Can tabular data have continuous values? what is meant by real, and how do we know it is a meaningful predictor? 
- <mark class="hltr-red">"Raw” data is unprocessed and has a complex data type”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=YD5I9DWL) 
- <mark class="hltr-blue">"with interactions”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=XAJLNWSK) 
	- what interactions in this context? Do the categories potentially have overlap themselves? 
- <mark class="hltr-blue">"complex interactions (i.e., more than quadratic”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=AL9QX5JS) 
	- What are complex interactions? 
- <mark class="hltr-blue">"small enough that they can be memorized by humans.”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=833SAWMN) 
	- What kind of data is easy to memorize by people? 
- <mark class="hltr-purple">"understood by humans. These constraints can differ dramatically depending on the domain.”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=AF4UNFQD) 
- <mark class="hltr-yellow">"min  f ∈F  1 n  ∑  i  Loss(f, zi) + C · InterpretabilityPenalty(f ), subject to (*)  InterpretabilityConstraint(f )”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=NB3Y9DVT) 
	- We choose a loss function (goal, quanitity/outcome to control) and select a model from a function class as defined by Table 1(?). 

If we increase the interpretability, we must assign a penalty for knowing the reasoning process.

The constraints are domain dependent. 
- <mark class="hltr-red">"soft and hard interpretability constraints”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=BQA2395E) 
	- define differences 
- <mark class="hltr-yellow">"(xi, yi), xi ∈ Rp, yi ∈ {−1, 1}”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=TA2C6Q8V) 
	- Example of data input and assigned label for supervised data item. In relation to (*) 
- <mark class="hltr-blue">"While solutions of (*) would not necessarily be sufficiently interpretable to use in practice, the constraints would generally help us find models that would be interpretable (if we design them well), and we might also be willing to consider slightly suboptimal solutions to find a more useful model.”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=47N64D66) 
	- Why is the solution set not fully interperetable? 
- <mark class="hltr-yellow">"C trades off between accuracy and the interpretability penalty”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=J7NTYF2N) 
	- modulates the outcome-- need subjectivity. 
- <mark class="hltr-blue">"Equation (*) can be generalized to unsupervised learning, where the loss term would simply be replaced by a loss term for the unsupervised problem, whether it is novelty detection, clustering, dimension reduction, or another task.”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=UURTFQT8) 
	- What is meant by modifiying the loss term? 
- <mark class="hltr-green">"Creating interpretable models can sometimes be much more difficult than creating black box models for many different reasons including:”</mark> [Page 4](zotero://open-pdf/library/items/SEK5XBGS?page=4&annotation=R4ZYIWGB) 
	- depends on model complexity (constraints), data processing leading to deployement slowdowns, uncertainity on definition of interpertability 
- <mark class="hltr-red">"This definition might require refinement, sometimes over multiple iterations with domain experts. There are many papers detailing these issues, the earliest dating from the mid-1990s [e.g., 157].”</mark> [Page 5](zotero://open-pdf/library/items/SEK5XBGS?page=5&annotation=AMPYWYWH) 
	- What drives the definition of interpertabilitiy from a domain level and from the CS community? 
- <mark class="hltr-purple">"157].”</mark> [Page 5](zotero://open-pdf/library/items/SEK5XBGS?page=5&annotation=WLC7WSIF) 
	- find issues with defining interpertability 
- <mark class="hltr-yellow">"accuracy, weighted accuracy, precision, average precision, precision@N, recall, recall@N, DCG, NCDG, AUC, partial AUC, mean-timeto-failure, etc.”</mark> [Page 5](zotero://open-pdf/library/items/SEK5XBGS?page=5&annotation=FAS5U4WP) 
	- metrics for performance. Int. has similar taxology. 
- <mark class="hltr-red">"Interpretability penalties or constraints can include sparsity of the model, monotonicity with respect to a variable, decomposibility into sub-models, an ability to perform case-based reasoning or other types of visual comparisons, disentanglement of certain types of information within the model’s reasoning process, generative constraints (e.g., laws of physics), preferences among the choice of variables, or any other type of constraint that is relevant to the domain”</mark> [Page 5](zotero://open-pdf/library/items/SEK5XBGS?page=5&annotation=7WG3E7LH) 
	- Need to understand why knowledge of these penalizes the outcome from (*) 
- <mark class="hltr-blue">"Choices of model form (e.g., the choice to use a decision tree, or a specific neural architecture) are examples of interpretability constraints.”</mark> [Page 5](zotero://open-pdf/library/items/SEK5XBGS?page=5&annotation=RU4MQEF4) 
	- How does choice of the model change the penalty? It is the input to the formula 
- <mark class="hltr-blue">"fully interpretable and partially interpretable models, often preferring the former”</mark> [Page 5](zotero://open-pdf/library/items/SEK5XBGS?page=5&annotation=4K8UU228) 
	- The choice of model partially drives the desirability of how interpretable it is. What factors of a model do we consider, and is there a tradeoff in the penalty term? would it be smaller where the desirability for fully interpretable models is high? 
- <mark class="hltr-blue">"decisions where an explanation would be trivial and the model is 100% reliable”</mark> [Page 5](zotero://open-pdf/library/items/SEK5XBGS?page=5&annotation=XXIXXXE2) 
	- Is this based on the classification/output of the model? does the model *need* 100% reliability? 
- <mark class="hltr-blue">"decisions where humans can verify or modify the decision afterwards”</mark> [Page 5](zotero://open-pdf/library/items/SEK5XBGS?page=5&annotation=68TFDYXH) 
	- Are there frameworks for assessing the reasoning that would benefit from having an interpretability metric?


Otherwise, how could we learn from *why* we modify the decision in the first place, and how we could alter the model later 
- <mark class="hltr-magenta">"Principle 2 Despite common rhetoric, interpretable models do not necessarily create or enable trust – they could also enable distrust. They simply allow users to decide whether to trust them. In other words, they permit a decision of trust, rather than trust itself.”</mark> [Page 6](zotero://open-pdf/library/items/SEK5XBGS?page=6&annotation=NAI7NB5N) 
	- How do we define a "reliable" decision maker? Perhaps there is something in affective theory to draw from here on what criteria we use to trust other people 
- <mark class="hltr-blue">"With black boxes, one needs to make a decision about trust with much less information; without knowledge about the reasoning process of the model”</mark> [Page 6](zotero://open-pdf/library/items/SEK5XBGS?page=6&annotation=I4ERE2YY) 
	- What frameworks do we use the evaluate a human's reasoning process? 
- <mark class="hltr-green">"here is no scientific evidence for a general tradeoff between accuracy and interpretability when one considers the full data science process for turning data into knowledge.”</mark> [Page 6](zotero://open-pdf/library/items/SEK5XBGS?page=6&annotation=RKMSW8CA) 
- <mark class="hltr-magenta">"interpretability often begets accuracy”</mark> [Page 6](zotero://open-pdf/library/items/SEK5XBGS?page=6&annotation=FDAY8ZU6) 
- <mark class="hltr-magenta">"no evidence of a general tradeoff of accuracy with interpretability.”</mark> [Page 7](zotero://open-pdf/library/items/SEK5XBGS?page=7&annotation=8MZYAIT9) 
	- is this domain dependent? 
- <mark class="hltr-purple">"COMPAS depends on race other than through age and criminal history [13, 258]”</mark> [Page 7](zotero://open-pdf/library/items/SEK5XBGS?page=7&annotation=W9TSNVCE) 
	- what does is mean by racial dependence? 
- <mark class="hltr-green">"The story of COMPAS is a key example simultaneously demonstrating many pitfalls of black boxes in practice. And, it shows an example of when black boxes are unnecessary, but used anyway.”</mark> [Page 7](zotero://open-pdf/library/items/SEK5XBGS?page=7&annotation=ZPSHA6FD) 
- <mark class="hltr-green">"ar domain is that of Afnan et al. [4], who discuss in vitro fertilization (IVF). In modern IVF, black box models that have not been subjected to randomized controlled trials determine who comes into existence”</mark> [Page 7](zotero://open-pdf/library/items/SEK5XBGS?page=7&annotation=86SD2DYE) 
	- very morally touchy subject. Relate to randomization and fairness 
- <mark class="hltr-green">"shared decision-making with patients”</mark> [Page 7](zotero://open-pdf/library/items/SEK5XBGS?page=7&annotation=ZRMMJMKP) 
- <mark class="hltr-green">"“Who is accountable when the model causes harm?””</mark> [Page 7](zotero://open-pdf/library/items/SEK5XBGS?page=7&annotation=RBBCWA4L) 
- <mark class="hltr-blue">"inflated by including many “obvious” cases”</mark> [Page 7](zotero://open-pdf/library/items/SEK5XBGS?page=7&annotation=2ZLGQYGM) 
	- Why are "obvious' cases misleading?
ROC- Distinguishability between classes 
- <mark class="hltr-purple">"hat do not sacrifice accuracy but gain substantial interpretability [333, 53, 158, 58, 12, 216]”</mark> [Page 8](zotero://open-pdf/library/items/SEK5XBGS?page=8&annotation=D9FN4RNQ) 
	- papers for intuition about accuracy and interpretability, and how on un-pre-processed datasets, we can get goof accuracy 
- <mark class="hltr-green">"In these domains, neural networks generally find no advantage.”</mark> [Page 8](zotero://open-pdf/library/items/SEK5XBGS?page=8&annotation=IJTHFINA) 
	- relate to rashomon set. Tabular data has good performance without blackbox methods. What would necessitate the trade off to obfsucate interpretability to choose a blackbox model? 
- <mark class="hltr-purple">"The fact that simple models perform well for tabular data could arise from the Rashomon Effect discussed by Leo Breiman [41].”</mark> [Page 8](zotero://open-pdf/library/items/SEK5XBGS?page=8&annotation=2JHQQIMJ) 
	- Rashomon Set and intepretability 
- <mark class="hltr-green">"In such cases, as discussed earlier and in Challenges 4 and 5, interpretable neural networks suffice, without losing accuracy.”</mark> [Page 8](zotero://open-pdf/library/items/SEK5XBGS?page=8&annotation=4SXVYDWY) 
	- there is no dichotomy (principle 3)- this is all dependent on the existence of the Rashomon set. Interpretable black box models could exist, and it may be dependent on the type of data the model is deployed on. (tabular vs. raw data). 
- <mark class="hltr-blue">"n interpretable robotic surgeon would be worse than its black box counterpart. The question ultimately becomes whether the Rashomon set should permit such an interpretable robotic surgeon–and all scientific evidence so far (including a large-and-growing number of experimental papers on interpretable deep learning) suggests it would.”</mark> [Page 9](zotero://open-pdf/library/items/SEK5XBGS?page=9&annotation=UYI4EFTZ) 
	- What do we mean by "worse"? Are we defining this in terms of accuracy? 
- <mark class="hltr-magenta">"Principle 4 As part of the full data science process, one should expect both the performance metric and interpretability metric to be iteratively refined.”</mark> [Page 9](zotero://open-pdf/library/items/SEK5XBGS?page=9&annotation=KUQNDW4F) 
- <mark class="hltr-magenta">"Principle 5 For high stakes decisions, interpretable models should be used if possible, rather than “explained” black box models.”</mark> [Page 9](zotero://open-pdf/library/items/SEK5XBGS?page=9&annotation=V357WN52) 
	- define interpretable versus explained 
- <mark class="hltr-blue">"Unfortunately, these topics are much too often lumped together within the misleading term “explainable artificial intelligence” or “XAI” despite a chasm separating these two concepts [250]”</mark> [Page 9](zotero://open-pdf/library/items/SEK5XBGS?page=9&annotation=LWVNQ6QH) 
	- Concretley state the argument between explainability and interpretability. Explainability seems to be the mathematical framework to understand the outcomes of the blackbox, whereas interpretable aims to made predictive models a human can make.


but this is still unclear 
- <mark class="hltr-magenta">"Explainability and interpretability techniques are not alternative choices for many real problems, as the recent surveys often imply; one of them (XAI) can be dangerous for high-stakes decisions to a degree that the other is not.”</mark> [Page 9](zotero://open-pdf/library/items/SEK5XBGS?page=9&annotation=IRUEYMG3) 
- <mark class="hltr-green">"uch issues with explanations have arisen with assessment of fairness and variable importance [258, 82] as well as uncertainty bands for variable importance [113, 97]”</mark> [Page 10](zotero://open-pdf/library/items/SEK5XBGS?page=10&annotation=JLRSFSQZ) 
	- What are uncertainty bands? 
- <mark class="hltr-green">"posthoc explanation, called saliency maps”</mark> [Page 10](zotero://open-pdf/library/items/SEK5XBGS?page=10&annotation=YEJAD72D) 
	- posthoc processing is not good 
- <mark class="hltr-blue">"A “saliency” real estate agent would say that the price is determined from the roof and backyard, but doesn’t explain how the roof and backyard were used to determine the price”</mark> [Page 10](zotero://open-pdf/library/items/SEK5XBGS?page=10&annotation=YFPB3XV8) 
	- gives example on what is meant by explaining function approximations 
- <mark class="hltr-green">"Typographical errors in input data are a prime example of this issue”</mark> [Page 10](zotero://open-pdf/library/items/SEK5XBGS?page=10&annotation=V9HEKUR4) 
- <mark class="hltr-purple">"Explainability techniques give authority to black box models rather than suggesting the possibility of models that are understandable in the first place [253]”</mark> [Page 11](zotero://open-pdf/library/items/SEK5XBGS?page=11&annotation=FT5MH46B) 
- <mark class="hltr-blue">"But function approximators are not used in interpretable ML; instead of approximating a known function (a black box ML model), interpretable ML can choose from a potential myriad of approximatelyequally-good models, which, as we noted earlier, is called “the Rashomon set””</mark> [Page 11](zotero://open-pdf/library/items/SEK5XBGS?page=11&annotation=LWZI7AK4) 
	- difference between model and function in this context 
- <mark class="hltr-purple">"But function approximators are not used in interpretable ML; instead of approximating a known function (a black box ML model), interpretable ML can choose from a potential myriad of approximatelyequally-good models, which, as we noted earlier, is called “the Rashomon set” [41, 97, 269]”</mark> [Page 11](zotero://open-pdf/library/items/SEK5XBGS?page=11&annotation=7ICAZ5TM) 
	- FA is for explainability(?). We cannot simply construct some equation based on function behavior alone, it must follow constraints from th erashomon set 
- <mark class="hltr-green">"an interpretable model is constrained, following a domain-specific set of constraints that make reasoning processes understandable.”</mark> [Page 11](zotero://open-pdf/library/items/SEK5XBGS?page=11&annotation=WSW3XDP2) 
- <mark class="hltr-green">"When would we use logical models? Logical models are usually an excellent choice for modeling categorical data with potentially complicated interaction terms”</mark> [Page 12](zotero://open-pdf/library/items/SEK5XBGS?page=12&annotation=46F97PA8) 
- <mark class="hltr-green">"These greedy methods for building decision trees create trees from the top down and prune them back afterwards. They do not go back to fix a bad split if one was made. Consequently, the trees created from these greedy methods tend to be both less accurate and less interpretable than necessary”</mark> [Page 12](zotero://open-pdf/library/items/SEK5XBGS?page=12&annotation=9PN2WKHT) 
	- relate to table 2 ,data types and models. this if for multiclass data and categorical data 
- <mark class="hltr-green">"This gap can cause a problem in practice because one does not know whether poor performance is due to the choice of model form (the choice to use a decision tree of a specific size) or poor optimization (not fully optimizing over the set of decision trees of that size).”</mark> [Page 13](zotero://open-pdf/library/items/SEK5XBGS?page=13&annotation=RAIWVI7C) 
- <mark class="hltr-yellow">"sparsity is measured by the number of leaves in the tree”</mark> [Page 14](zotero://open-pdf/library/items/SEK5XBGS?page=14&annotation=N6M2JBNS) 
- <mark class="hltr-green">"Can we improve the scalability of optimal sparse decision trees?”</mark> [Page 14](zotero://open-pdf/library/items/SEK5XBGS?page=14&annotation=BAUI2ZXP) 
	- accuracy and sparsity are two challenging areas for decision trees 
- <mark class="hltr-green">"Can we efficiently handle continuous variables?”</mark> [Page 15](zotero://open-pdf/library/items/SEK5XBGS?page=15&annotation=S4L2Y9JA) 
- <mark class="hltr-green">"These methods are unable to jointly optimize the selection of variables to split at each internal tree node, the splitting threshold of that variable (if it is continuous), and the tree structure (the overall shape of the tree). Lin et al”</mark> [Page 15](zotero://open-pdf/library/items/SEK5XBGS?page=15&annotation=YJUIZH3W) 
- <mark class="hltr-green">"Can we handle constraints more gracefully?”</mark> [Page 16](zotero://open-pdf/library/items/SEK5XBGS?page=16&annotation=C67VD4GP) 
- <mark class="hltr-red">"coring systems are linear classification models that require users to add, subtract, and multiply only a few small numbers in order to make a prediction.”</mark> [Page 16](zotero://open-pdf/library/items/SEK5XBGS?page=16&annotation=CZCFM8UG) 
- <mark class="hltr-green">"Each scoring system was created using a different method involving different heuristics. Some of them were built using domain expertise alone without data, and some were created using rounding heuristics for logistic regression coefficients and other manual feature selection approaches to obtain integer-valued point scores [see, e.g., 175].”</mark> [Page 17](zotero://open-pdf/library/items/SEK5XBGS?page=17&annotation=SYX3N3KW) 
- <mark class="hltr-green">"When rounding, we lose all signal coming from all variables except the first two. The contribution from the eliminated variables may together be significant even if each individual coefficient is small, in which case, we lose predictive performance.”</mark> [Page 18](zotero://open-pdf/library/items/SEK5XBGS?page=18&annotation=QZVFCGIX) 
- <mark class="hltr-green">"1 regularization does more than make the solution sparse, it also imposes a strong 1 bias.”</mark> [Page 18](zotero://open-pdf/library/items/SEK5XBGS?page=18&annotation=56NFXGVB) 
- <mark class="hltr-green">"Some of these constraints may be able to be placed into the mathematical program, but it is still not clear whether the solution of the optimization problem one solves would actually be close to the solution of the optimization problem we actually care about.”</mark> [Page 19](zotero://open-pdf/library/items/SEK5XBGS?page=19&annotation=DLINRWWL) 
- <mark class="hltr-green">"Improve the scalability of optimal sparse scoring systems: As discussed, for scoring systems, the only practical approaches that produce optimal scoring systems require a MIP solver, and these approaches may not be able to scale to large problems, or optimally handle continuous variables”</mark> [Page 20](zotero://open-pdf/library/items/SEK5XBGS?page=20&annotation=VQ368IK3) 
	- solutions 
- <mark class="hltr-green">"Improve the scalability of optimal sparse scoring systems: As discussed, for scoring systems, the only practical approaches that produce optimal scoring systems require a MIP solver, and these approaches may not be able to scale to large problems, or optimally handle continuous variables.”</mark> [Page 20](zotero://open-pdf/library/items/SEK5XBGS?page=20&annotation=IH5RG3DF) 
- <mark class="hltr-green">"Ease of constraint elicitation and handling:”</mark> [Page 20](zotero://open-pdf/library/items/SEK5XBGS?page=20&annotation=2BU86P2I) 
- <mark class="hltr-green">"For instance, if we had better ways of representing and exploring the Rashomon set (see Challenge 9), domain experts might be able to search within it effectively, without fear of leaving that set and producing a suboptimal model.”</mark> [Page 20](zotero://open-pdf/library/items/SEK5XBGS?page=20&annotation=M6TGLWIP) 
- <mark class="hltr-green">"importance of features, we should be able to incorporate that through regularization [307].”</mark> [Page 21](zotero://open-pdf/library/items/SEK5XBGS?page=21&annotation=79ZY87JP) 
- <mark class="hltr-blue">"linear models, which includes scoring systems (and risk scores)”</mark> [Page 21](zotero://open-pdf/library/items/SEK5XBGS?page=21&annotation=729DPMNN) 
	- linear models are logical models? 
- <mark class="hltr-yellow">"g(E[y]) = β0 + f1(x·1) + ... + fp(x·p),”</mark> [Page 21](zotero://open-pdf/library/items/SEK5XBGS?page=21&annotation=BS7FL9WH) 
	- generative additive model 
- <mark class="hltr-green">"Fig 4. Hierarchical relationships between GAMs, additive models, linear models, and scoring systems.”</mark> [Page 22](zotero://open-pdf/library/items/SEK5XBGS?page=22&annotation=QEAUTEWT) 
- <mark class="hltr-blue">"The standard form of GAMs is interpretable because the model is constrained to be a linear combination of univariate component functions.”</mark> [Page 22](zotero://open-pdf/library/items/SEK5XBGS?page=22&annotation=88FCURWL) 
	- This is a deterministic function-- different than function approximation 
- <mark class="hltr-yellow">"fj (x·j ) =  ∑  thresholdsj′  cj,j′ 1[x·j &gt; θj′ ].”</mark> [Page 23](zotero://open-pdf/library/items/SEK5XBGS?page=23&annotation=BU3TANNQ) 
	- sum of component functions. 
- <mark class="hltr-blue">"boosted models are not naturally sparse, and issues with bias arise under 1 regularization, as discussed in the scoring systems section.”</mark> [Page 23](zotero://open-pdf/library/items/SEK5XBGS?page=23&annotation=47FY85LE) 
	- What are proxies? Connects to how regularizaiton issues (stripping away too many small weights) if tree is not sparse can be an issue. 
- <mark class="hltr-green">"sparsity in the number of component functions and smoothness of the component functions”</mark> [Page 23](zotero://open-pdf/library/items/SEK5XBGS?page=23&annotation=3PIXXEDZ) 
	- Main ways to control GAM interpetability 
- <mark class="hltr-green">"1 regularization imposes a strong unintended bias on the coefficients when aiming for very sparse solutions. (2) Lou et al. [195] find that imposing smoothness may come at the expense of accuracy, (3)”</mark> [Page 24](zotero://open-pdf/library/items/SEK5XBGS?page=24&annotation=98M9GWZQ) 
	- main issue with regularization and accuracy again 
- <mark class="hltr-green">"GAMs are often used on raw medical records or other complex data types, and these datasets are likely to benefit from troubleshooting.”</mark> [Page 24](zotero://open-pdf/library/items/SEK5XBGS?page=24&annotation=KN5GPSZ5) 
	- model used for raw data type. good at finding patterns in data or missing relationships. Broadest class that can be distilled down into morte speciifc models like decisons trees or scoring systems by controlling sparsity, monotonicity, and smoothness 
- <mark class="hltr-red">"Case-based reasoning is a paradigm that involves solving a new problem using known solutions to similar past problems [1]. It is a problem-solving strategy that we humans use naturally in our decision-making processes [219]”</mark> [Page 25](zotero://open-pdf/library/items/SEK5XBGS?page=25&annotation=GLY6YGDE) 
- <mark class="hltr-green">"case-based reasoning applies to both tabular and raw data, including computer vision.”</mark> [Page 25](zotero://open-pdf/library/items/SEK5XBGS?page=25&annotation=3A4S9C6Q) 
- <mark class="hltr-green">"There are, in general, two types of case-based reasoning techniques: (i) nearest neighbor-based techniques, and (ii) prototype-based techniques”</mark> [Page 25](zotero://open-pdf/library/items/SEK5XBGS?page=25&annotation=K2IVJ29V) 
- <mark class="hltr-red">"Nearest neighbor-based techniques. These techniques make a decision for a previously unseen test instance, by finding training instances that most closely resemble the particular test instance”</mark> [Page 26](zotero://open-pdf/library/items/SEK5XBGS?page=26&annotation=MU57BMYL) 
- <mark class="hltr-blue">"using a deep neural network that transforms the input space into a feature space where a kNN classifier will perform well (i.e., deep kNN). Papernot and McDaniel [229]”</mark> [Page 26](zotero://open-pdf/library/items/SEK5XBGS?page=26&annotation=JM7LZQVU) 
	- what is the relation to latent spaces here? 
- <mark class="hltr-green">"those techniques often require a substantial amount of distance computations (e.g., to find out the nearest neighbors of a test input), which can be slow in practice. Also, it is possible that the nearest neighbors may not be particularly good representatives of a class, so that reasoning about nearest neighbors may not be interpretable”</mark> [Page 27](zotero://open-pdf/library/items/SEK5XBGS?page=27&annotation=8A3NQA4X) 
- <mark class="hltr-red">"Given a previously unseen test instance, they make a decision by finding prototypical cases (instead of training instances from the entire training set) that most closely resemble the particular test instance”</mark> [Page 27](zotero://open-pdf/library/items/SEK5XBGS?page=27&annotation=FLRVILJY) 
- <mark class="hltr-yellow">"During training, if the training example’s class agrees with the nearest prototype’s class, then the prototype is moved closer to the training example; otherwise the prototype is moved further away from the training example.”</mark> [Page 27](zotero://open-pdf/library/items/SEK5XBGS?page=27&annotation=DSKALA5Y) 
	- method for how prototype reasoning works 
- <mark class="hltr-green">"Part-based prototypes. One issue that arises with both nearest neighbor and prototype techniques is the comparison of a whole observation to another whole observation.”</mark> [Page 27](zotero://open-pdf/library/items/SEK5XBGS?page=27&annotation=R3WRI2MN) 
- <mark class="hltr-purple">"More recently, Chen et al. [53] extended the work of Li et al. [183] to create a prototypical part network (ProtoPNet) whose prototype layer stores proto Interpretable machine learning grand challenges 29  typical parts of encoded training images. The prototypical parts are patches of convolutional-neural-network-encoded training images, and represent typical features observed for various image classes. Given an input instance, the network compares an encoded input image with each of the learned prototypical parts, and generates a prototype activation map that indicates both the location and the degree of the image patch most similar to that prototypical part. The authors applied the network to the benchmark Caltech-UCSD Birds-200-2011 (CUB-200-2011) dataset [305] for bird recognition, and the ProtoPNet was able to learn prototypical parts of 200 classes of birds, and use these prototypes to classify birds with an accuracy comparable to non-interpretable black-box models.”</mark> [Page 28](zotero://open-pdf/library/items/SEK5XBGS?page=28&annotation=PSEHIAV5) 
- <mark class="hltr-green">"? Currently, case-based reasoning has been used for structured (tabular) data, static images, and simple sequences such as text.”</mark> [Page 29](zotero://open-pdf/library/items/SEK5XBGS?page=29&annotation=5W6JRMPG) 
- <mark class="hltr-green">"Current approaches to prototype learning do not take into account prior knowledge or expert opinions. At times, it may be advantageous to develop prototype-learning algorithms that collaborate with human experts in choosing prototypical cases or prototypical features”</mark> [Page 30](zotero://open-pdf/library/items/SEK5XBGS?page=30&annotation=L77METCB) 
- <mark class="hltr-blue">"prototype-learning algorithms that collaborate with human experts in choosing prototypical cases or prototypical features. For example, in healthcare, it would be beneficial if a prototype-based classifier learns, under the supervision of human doctors”</mark> [Page 30](zotero://open-pdf/library/items/SEK5XBGS?page=30&annotation=9FGB6R9W) 
- <mark class="hltr-red">"Disentanglement” here refers to the way information travels through the network: we would perhaps prefer that all information about a specific concept (say “lamps”) traverse through one part of the network while information about another concept (e.g., “airplane”) traverse through a separate part.”</mark> [Page 31](zotero://open-pdf/library/items/SEK5XBGS?page=31&annotation=XJXAPNYM) 
- <mark class="hltr-green">"n other words, using these constraints, we could constrain our network to have the kind of “Grandmother node” that scientists have been searching for in both real and artificial convolutional neural networks [115].”</mark> [Page 31](zotero://open-pdf/library/items/SEK5XBGS?page=31&annotation=SBGN6MEG) 
- <mark class="hltr-green">"n that sense, vectors in the latent space are “impure” in that they do not naturally represent single concepts [see 58, for a detailed discussion].”</mark> [Page 32](zotero://open-pdf/library/items/SEK5XBGS?page=32&annotation=CY7BEST3) 
	- we align the axis of the neurons along latent spaces of classes- loading the concepts may take a lot of time if the network has a lot of neurons 
- <mark class="hltr-green">"but this would not mean that the information flow concerning each concept goes only though that concept’s designated path through the network;”</mark> [Page 33](zotero://open-pdf/library/items/SEK5XBGS?page=33&annotation=79G3A6BT) 
- <mark class="hltr-green">"Perhaps the latter problem could be solved by training with a small random subset of concepts at each iteration; but this has not been tried in current methods at the time of this writing.”</mark> [Page 33](zotero://open-pdf/library/items/SEK5XBGS?page=33&annotation=N5CYJ86G) 
- <mark class="hltr-green">"How to choose good concepts to learn for disentanglement?”</mark> [Page 34](zotero://open-pdf/library/items/SEK5XBGS?page=34&annotation=224AU3E5) 
- <mark class="hltr-green">"The decision process of current disentangled neural networks contains two parts, x → c mapping the input x to the disentangled representation (concepts) c, and c → y mapping the disentangled representation c to the output y.”</mark> [Page 34](zotero://open-pdf/library/items/SEK5XBGS?page=34&annotation=D6AK8MMK) 
	- there is a gap bc the last output layer is still a blackbox 
- <mark class="hltr-green">"pretability of the latent space and the interpretability of the entire model. Current methods either rely on variable importance methods to explain c → y posthoc [58], or simply make c → y a linear layer [158].”</mark> [Page 35](zotero://open-pdf/library/items/SEK5XBGS?page=35&annotation=3Q5T8V8A) 
	- use var. importance or posthoc explanations 
- <mark class="hltr-green">"But in the case where we do not know the concepts, or in the case where the concepts are numerous and we do not know how to parameterize them, we cannot use the techniques from Challenge 5. In other words, the concept c in Constraint (5.1) is no longer a concept we predefine, but it must still be an actual concept in the existing universe of concepts”</mark> [Page 35](zotero://open-pdf/library/items/SEK5XBGS?page=35&annotation=7DW9AIFH) 
	- we do not know the classes ahead of time unlike other case. Makes quantitavely evaluating harder if we know nothing about the classes. we may also ignore key iunformaiton if we have human annotators. 
- <mark class="hltr-green">"abeled datasets for computer vision have a severe labeling bias: we tend only to label entities in images that are useful for a specific task (e.g., object detection), thus ignoring much of the information found in images.”</mark> [Page 36](zotero://open-pdf/library/items/SEK5XBGS?page=36&annotation=JM3478CN) 
- <mark class="hltr-green">"Chen et al. [53] propose to create a prototype layer, storing prototypical parts of training images, to do case based reasoning. When classifying birds, the prototypical parts are usually object parts such as heads and wings of birds.”</mark> [Page 38](zotero://open-pdf/library/items/SEK5XBGS?page=38&annotation=EWBW9XK8) 
	- connection between case based reasoning and disentangelemnt to tie back to interpretability of concepts 
- <mark class="hltr-green">"unsupervised disentanglement is desired (but challenging) in two different types of domains: (a) domains in which we do not know what the concepts are (e.g., materials science); (b) domains in which concepts are known but labeling biases exist.”</mark> [Page 39](zotero://open-pdf/library/items/SEK5XBGS?page=39&annotation=4U46X6LW) 
- <mark class="hltr-blue">"part-whole disentanglement for more complicated patterns in large vision datasets?”</mark> [Page 40](zotero://open-pdf/library/items/SEK5XBGS?page=40&annotation=6H5PH89S) 
	- same relation to part-based breakdown as in case- based models with prototypical models. 
- <mark class="hltr-green">"enerally speaking, there are two primary types of approaches to DR for visualization, commonly referred to as local and global methods. Global methods aim mainly to preserve distances between any pair of points (rather than neighborhoods), while the local methods emphasize preservation of local neighborhoods (that is, which points are nearest neighbors).”</mark> [Page 41](zotero://open-pdf/library/items/SEK5XBGS?page=41&annotation=FJMNK5LM) 
- <mark class="hltr-green">"distances from the original space when creating low-dimensional embeddings. But distances between points behave differently in high dimensions than in low dimensions, leading to problems preserving the distances.”</mark> [Page 42](zotero://open-pdf/library/items/SEK5XBGS?page=42&annotation=AGLXZZ9V) 
	- also dependent on assumptions about the accuracy of distance metric for data-- not god for neuron weights. not choosing  which hyperparameters are important can lead to loss of global data. 
- <mark class="hltr-green">"When their perplexity parameter or the number of nearest neighbors is not chosen carefully, algorithms can fail to preserve the global structure of the mammoth (specifically, the overall placement of the mammoth’s parts), and they create spurious clusters (losing connectivity between parts of the mammoth) and lose details (such as the toes on the feet of the mammoth)”</mark> [Page 44](zotero://open-pdf/library/items/SEK5XBGS?page=44&annotation=MPT9Q59Q) 
- <mark class="hltr-green">"It may be useful to design modern approaches to help users understand how the final two or three dimensions are defined in terms of the high-dimensional features”</mark> [Page 44](zotero://open-pdf/library/items/SEK5XBGS?page=44&annotation=G259XGR4) 
	- not really a god way at the moment to understand PCA and other techniques-- too much complexity for a human. focus on defining realtionships from high dimensional feature to final data with posthoc interpretations. 
- <mark class="hltr-blue">"This may take the form of explanatory post-hoc visualizations or constrained DR methods.”</mark> [Page 44](zotero://open-pdf/library/items/SEK5XBGS?page=44&annotation=TBHJ8VBI) 
	- idea: when us post-hoc or in the loop human decision making for iteratiove model updates better? 
- <mark class="hltr-red">"n general, a PINN is a neural network that approximates the solution of a set of PDEs with initial and boundary conditions. The training of a PINN minimizes the residuals from the PDEs as well as the residuals from the initial and boundary conditions.”</mark> [Page 46](zotero://open-pdf/library/items/SEK5XBGS?page=46&annotation=CN29XNSA) 
	- constraints based on laws of nature, PDE/ODES for material science, etc. 
- <mark class="hltr-yellow">"he derivative g′(t) with respect to input t (at each of those finitely many points t used for training) is found by leveraging the existing network structure of g using back-propagation”</mark> [Page 46](zotero://open-pdf/library/items/SEK5XBGS?page=46&annotation=YB68NZ9X) 
- <mark class="hltr-green">"Currently, data that might be used for training PINNs are often collected (from experiments or simulations) beforehand (i.e., prior to training of PINNs). This could lead to large uncertainty bands on areas of the input domain where data are scarce, and when the parameters of the PDE need to be learned from these data.”</mark> [Page 47](zotero://open-pdf/library/items/SEK5XBGS?page=47&annotation=7I6AVZCC) 
- <mark class="hltr-purple">"Knowledge graphs encode relationships between entities in the world, including common sense knowledge. Thus, being able to incorporate information from a knowledge graph could be very helpful if we can figure out ways to do it effectively.”</mark> [Page 48](zotero://open-pdf/library/items/SEK5XBGS?page=48&annotation=TJAZHZEV) 
- <mark class="hltr-red">"The Rashomon effect occurs when there are multiple descriptions of the same event [41] with possibly no ground truth”</mark> [Page 48](zotero://open-pdf/library/items/SEK5XBGS?page=48&annotation=7R89QVFH) 
- <mark class="hltr-green">"neural networks that perform case-based reasoning on disentanglement still yielded models that were equally accurate to their unconstrained values; thus, these interpretable deep neural models are within the Rashomon set”</mark> [Page 49](zotero://open-pdf/library/items/SEK5XBGS?page=49&annotation=3HHFJ3DR) 
- <mark class="hltr-yellow">"R(F , f ∗, ) = {f ∈ F such that Loss(f ) ≤ Loss(f ∗) + },”</mark> [Page 49](zotero://open-pdf/library/items/SEK5XBGS?page=49&annotation=QAH3UA9R) 
- <mark class="hltr-green">"think of this as high-dimensional polynomials that are complex enough to fit the data well without overfitting). If a set of simpler functions Fsimpler could serve as approximating set for Fcomplicated (think decision trees of a certain depth approximating the set of polynomials), it means that each complicated function could be well-approximated by a simpler function (and indeed, polynomials can be well-approximated by decision trees). By this logic, the ball of Fcomplicated that is within the Rashomon set must contain at least one function within Fsimpler, which is the simple function we were looking for.”</mark> [Page 49](zotero://open-pdf/library/items/SEK5XBGS?page=49&annotation=MKVHDENS) 
	- basically, if we choose model class that doesnt over fit too mich we always have the sipler model we want thats accirate enought (defined by loss threshold) 
- <mark class="hltr-green">"Models with various important properties besides interpretability can exist in the Rashomon set, including fairness [67] and monotonicity”</mark> [Page 50](zotero://open-pdf/library/items/SEK5XBGS?page=50&annotation=HVA24C5Z) 
- <mark class="hltr-green">"size of the Rashomon set can be considered as a way of measuring the complexity of a learning problem.”</mark> [Page 50](zotero://open-pdf/library/items/SEK5XBGS?page=50&annotation=9I9EN9SI) 
- <mark class="hltr-blue">"e size of the Rashomon set differs from all of these quantities in fundamental ways, and it is important in its own right for showing the existence of simpler models.”</mark> [Page 50](zotero://open-pdf/library/items/SEK5XBGS?page=50&annotation=ES8W8MLE) 
	- fundemn 
- <mark class="hltr-green">"The Rashomon set can be represented as a subset of this variable importance space”</mark> [Page 50](zotero://open-pdf/library/items/SEK5XBGS?page=50&annotation=XPIACRUN) 
	- we can set the hypothesis with a latent space of variable importance for models, and see how reliant this variable is across models. 
- <mark class="hltr-red">"computing statistics of the Rashomon set in parameter space, such as the volume in parameter space, which is called the Rashomon volume”</mark> [Page 51](zotero://open-pdf/library/items/SEK5XBGS?page=51&annotation=N38NV5AP) 
- <mark class="hltr-green">"Overparametrization or underparametrization can cause volumes in parameter space to be artificially made larger or smaller without a change in the actual space of functions [83]. For instance, if we make a copy of a variable and include it in the datasets, it can change the Rashomon ratio.”</mark> [Page 51](zotero://open-pdf/library/items/SEK5XBGS?page=51&annotation=7NEYXJSF) 
- <mark class="hltr-green">"At worst, computation over the Rashomon set requires a brute force calculation over a large discrete hypothesis space. In most cases, the computation should be much easier. Perhaps we could use dynamic programming or branch and bound techniques to reduce the search space so that it encompasses the Rashomon set but not too much more than that?”</mark> [Page 53](zotero://open-pdf/library/items/SEK5XBGS?page=53&annotation=8VGEYXK9) 
	- how to find it 
- <mark class="hltr-green">"The success of these techniques most likely will have to depend on whether we can design a good metric for the model class”</mark> [Page 53](zotero://open-pdf/library/items/SEK5XBGS?page=53&annotation=NRRQHU95) 
- <mark class="hltr-green">"Can a similar framework that searches the Rashomon set, instead of the whole hypothesis space, be designed?”</mark> [Page 54](zotero://open-pdf/library/items/SEK5XBGS?page=54&annotation=4CZ3TUMU) 


> [!context]
> ==(How this article relates to other work in the field; how it ties in with key issues and findings by others, including yourself)==
> context:: 

> [!significance]
> ==(to the field; in relation to your own work)==
> significance:: 


## <h2 class="color-faded1">This is the faded color 1 (faded-red)</h2>

## <h2 class="color-faded2">This is the faded color 2 (faded-green)</h2>

## <h2 class="color-faded3">This is the faded color 3 (faded-yellow)</h2>

## <h2 class="color-faded4">This is the faded color 4 (faded-blue)</h2>

## <h2 class="color-faded5">This is the faded color 5 (faded-purple)</h2>

## <h2 class="color-faded6">This is the faded color 6 (faded-aqua)</h2>

## <h2 class="color-faded7">This is the faded color 7 (faded-orange)</h2>

