###### [home](/index.html)
## Horizontal Shear Capacity of Concrete Joints

It's often infeasible to pour a concrete structural element all at one time. Because of this, pours are often split up - the contractor may pour foundation grade beams, and then back and pour the slab on top. Or they may set a precast concrete floor, and then pour a concrete topping over them. Differently timed concrete pours will leave horizontal joints in through the concrete, creating a composite member.

Because horizontal shear will be transferred across this joint, it's necessary to know it's capacity to resist load. These provisions for calculating its capacity are given in ACI 318-19 Table 16.4.4.2:

![table16442](table16442.PNG)\

The code gives a severe penalty to concrete without shear reinforcing crossing the joint, and to concrete not roughened to a +-1/4" amplitude (with a roughened surface being required for an unreinforced joint). The maximum capacity of an unreinforced concrete joint is 80 psi.

Roughening a concrete surface to 1/4" amplitude and installing shear reinforcing are both labor-intensive, time consuming and costly. So it's useful to examine the source of this provision, particularly the 80 psi value for an unreinforced joint.

---

According the the commentary, these load capacities are based on research done in the early 60's:

![R16442](R16442.PNG)\

However, looking at these sources makes it unclear where the 80 psi comes from.

[Kaar (1960)](https://www.concrete.org/publications/internationalconcreteabstractsportal.aspx?m=details&ID=51685340) ran no tests for horizontal shear through unreinforced joints.

[Hanson (1960)](https://www.concrete.org/publications/internationalconcreteabstractsportal.aspx?m=details&ID=19425) states:

>3. The girder and push-off tests reported herein indicate a maximum shearing stress for composite action of 500 psi for a rough bonded surface and 300 psi for a smooth bonded surface. The compressive strengths of the concretes were 3000 and 5000 psi for the slab and girder, respectively.

And [Saemann and Washa (1964)](https://www.concrete.org/publications/internationalconcreteabstractsportal/m/details/id/16707) give an equation based on % steel, shear span, and effective depth, with unreinforced joint capacity ranging from 450psi to 200psi:

![saemann1964](saemann1964.PNG)\

So where does the 80psi value come from?

---

If we dig back, we find that this 80 psi value is very near the lower bound value of 78 psi that first appears in a report from ACI-ASCE Committee 333 in its 1960 report:

![aci333](aci333.PNG)\

78 psi is the given horizonal shear strength of specimen A2 (though its worth noting that all the unreinforced joints had a smooth surface). The committee used this data to recommend a bond value of 80 psi for smooth surfaces:

![aci333_2](aci333_2.PNG)\

The 80 psi value was incorporated into ACI 318-71 for both smooth reinforced and rough reinforced, and have been unchanged ever since:

![aci333_3](aci333_3.PNG)\

The source of A2 is reference 9, "Behavior of Composite Lintel Beams in Bending" Ozell (1956). This publication is currently unavailable from PCI, however, we can find it discussed in a CTA Technical Bulletin from 1974:

![CTA74](CTA74.PNG)\

The value of 78 psi seems to have been copied incorrectly. In fact, nearly all the values from table 2 are different than their original source:

![CTA74_2](CTA74_2.PNG)\

There is no source of the 80 psi value for horizontal shear - it's inclusion is due to a typo made 60 years ago.

---

So if the value of 80 psi is based on nothing, what is the actual capacity of an unreinforced horizontal concrete joint?

The research in this area is summarized in [Kovach (2008):](https://preserve.lehigh.edu/cgi/viewcontent.cgi?article=2018&context=etd)

![kovach2008](kovach2008.PNG)\
![kovach2008_2](kovach2008_2.PNG)\

The samples vary in concrete strength, surface finish, testing conditions, and preparation prior to pouring (with some being deliberately fabricated in such a way to prevent a bond from forming), making it difficult to draw direct conclusions beyond the obvious conservatism of the 80 psi limit.

Running his own series of tests, Kovach achieves the following results:

![kovach2008_3](kovach2008_3.PNG)\
![kovach2008_4](kovach2008_4.PNG)\

The horizontal shear strengths of an unreinforced joint as calculated by Kovach (and consistent with previous research) are 6-10 times that of the value currently required by ACI. 

Given the existing provisions provenance, and the results of more recent research, ACI should consider re-examining these provisions.

---

### References:

1. ACI 318-19
2. ACI-ASCE Committee 333 (1960). Tentative Recommendations for Design of Composite Beams and Girders, for Buildings. ACI Journal, 57(6), 609 - 628.
3. Concrete Technology Associates (1974). Composite Systems without Roughness. Technical
Bulletin 74-B6.
4. Hanson, N. W. (1960). Precast-Prestressed Concrete Bridges(2) Horizontal Shear Connections. Journal of the Research and Development Laboratories, Portland Cement Association, 2(2), 38 - 58.
5. Kaar, P. H.; Kriz, L. B.; and Hognestad, E., 1960, “PrecastPrestressed Concrete Bridges: (1) Pilot Tests of Continuous Girders,” Journal, PCA Research and Development Laboratories, V. 2, No. 2, May, pp. 21-37.
6. Kovach, J.D, 2008, "Horizontal Shear Capacity ofComposite Concrete Beams without Interface Ties", Masters Thesis, Lehigh University
7. Saemann, J. C., and Washa, G. W., 1964, “Horizontal Shear Connections between Precast Beams and Cast-in Place Slabs,” ACI Journal Proceedings, V. 61, No. 11, Nov., pp. 1383-1409. Also see discussion, ACI Journal Proceedings, V. 62, June 1965.

###### *last updated: 5/11/20*




