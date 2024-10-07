

### d-Separation

In causal diagrams, d-separation is a graphical criterion used to determine whether a set of variables is independent of another set, given a third set, based on the structure of the graph. A path between two variables is considered blocked or d-separated if, given the variables we condition on, the path does not transmit any association between the variables. If all paths between two variables are blocked, the variables are d-separated and are conditionally independent. Conversely, if any path is unblocked (d-connected), the variables may be dependent [@pearl1995; @pearl2009a]. Note that the “d” in d-separation stands for "directional."

Briefly stated, the rules of d-separation are as follows:

1.	Fork (Common Cause):
Diagram: $B \leftarrow \boxed{A} \rightarrow C$

Implication: conditioning on the common cause  $A$  blocks the association between  $B$  and  $C$ . Therefore,  $B$  and  $C$  are independent given  $A$ :
 
 $$
 B \coprod C \mid A
 $$ 

2.	Chain (Mediator):
Diagram: $A \rightarrow \boxed{B} \rightarrow C$

Implication: conditioning on the mediator  $B$  blocks the association between  $A$  and  $C$ . Thus,  $A$ and  $C$  are independent given  $B$ :
 $$
 A \coprod C \mid B
 $$

3.	Collider (Common Effect):
Diagram: $A \rightarrow \boxed{C} \leftarrow B$

Implication: conditioning on the common effect  $C$  (or any of its descendants) opens the path between  $A$  and  $B$ , introducing dependence. Hence,  $A$  and  $B$  are dependent given $C$:

$$
A \cancel \coprod \mid C
$$



It follows from d-separation that:

	1.	Colliders block paths when unconditioned: an open path (with no variables conditioned on) is blocked if it contains a collider— a node where two arrows converge. For example, in the diagram ￼, the node ￼ is a collider. This structure blocks any association between ￼ and ￼ when no variables are conditioned on.
	2.	Conditioning on a Collider Opens the Path: conditioning on a collider opens a previously blocked path, potentially introducing an association between variables that are not causally related. In the diagram $A \rightarrow \boxed{C} \leftarrow B$, conditioning on ￼ allows information to flow between ￼ and ￼, leading to a possible association in the absence of a direct causal link.
	3.	Conditioning on a descendant of a collider also opens the path: conditioning on a descendant of a collider has a similar effect. If ￼ and we condition on ￼, the path $A \rightarrow C \rightarrow \boxed{C{\prime}} \leftarrow B$ becomes unblocked. Thus, conditioning on ￼ opens the path between ￼ and ￼ through the collider ￼.
	4.	Conditioning on non-collider nodes blocks the path: if a path does not contain a collider, conditioning on any variable along that path blocks it. For instance, in the diagram $A \rightarrow \boxed{B} \rightarrow C$, conditioning on ￼ blocks the path from ￼ to ￼, rendering ￼ and ￼ conditionally independent given ￼ [@pearl2009a; @hernan2024WHATIF, p. 78].

These principles underscore the importance of understanding the structure of causal graphs when determining conditional independence and the flow of associations.  Judea Pearl developed and formalised the concept of d-separation in the 1990s [@pearl1995; @pearl2009a].