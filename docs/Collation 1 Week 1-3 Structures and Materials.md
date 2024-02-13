
> [!WARNING] Preprint version!!!
> This copy of Collation 1 Week 1-3 for Structures and Materials has not been fully peer reviewed by seniors and our cohort mates who are already familiar in this topic. While the author has made every possible effort to ensure correctness of information, this document might not be entirely accurate. 

**Version 0.1**

This collation is written in close reference to James F. Shackelford's Introduction to Materials Science for Engineers (2014 edition), and extensively uses images from this textbook. 

**Table of contents**
- [[#Classification of Materials|Classification of Materials]]
- [[#Chemical Bonding|Chemical Bonding]]
	- [[#Chemical Bonding#Bond Energy and Length|Bond Energy and Length]]
	- [[#Chemical Bonding#Primary Bonds|Primary Bonds]]
		- [[#Primary Bonds#Ionic bond|Ionic bond]]
			- [[#Ionic bond#Coordination Number (CN)|Coordination Number (CN)]]
		- [[#Primary Bonds#Covalent bond|Covalent bond]]
		- [[#Primary Bonds#Metallic bond|Metallic bond]]
	- [[#Chemical Bonding#Secondary Bonds|Secondary Bonds]]
- [[#Types of crystal structures|Types of crystal structures]]
- [[#Miller Indices|Miller Indices]]
	- [[#Miller Indices#Positional indices|Positional indices]]
	- [[#Miller Indices#Directional indices|Directional indices]]
	- [[#Miller Indices#Planar indices|Planar indices]]
- [[#Crystal Defects|Crystal Defects]]
	- [[#Crystal Defects#Solid solutions and hardening|Solid solutions and hardening]]
	- [[#Crystal Defects#Point Defects|Point Defects]]
	- [[#Crystal Defects#Interstitial Solutions|Interstitial Solutions]]
	- [[#Crystal Defects#Linear defects|Linear defects]]
	- [[#Crystal Defects#Planar defects|Planar defects]]
	- [[#Crystal Defects#Shape memory effect in NiTi|Shape memory effect in NiTi]]
- [[#Example of an Mg-Al system|Example of an Mg-Al system]]
- [[#Definition of Stress and Strain|Definition of Stress and Strain]]
- [[#Stress-Strain Relationship Curve|Stress-Strain Relationship Curve]]
- [[#Data from Tensile Testing|Data from Tensile Testing]]
	- [[#Data from Tensile Testing#Young's Modulus|Young's Modulus]]
		- [[#Young's Modulus#Bond stiffness|Bond stiffness]]
		- [[#Young's Modulus#Valence electron density and $E$|Valence electron density and $E$]]
	- [[#Data from Tensile Testing#Yield Strength|Yield Strength]]
	- [[#Data from Tensile Testing#Ultimate Tensile Strength|Ultimate Tensile Strength]]
	- [[#Data from Tensile Testing#Total % elongation / Ductility|Total % elongation / Ductility]]
- [[#Types of Stress and Strain|Types of Stress and Strain]]
	- [[#Types of Stress and Strain#Normal stress|Normal stress]]
	- [[#Types of Stress and Strain#Shear stress, strain and modulus|Shear stress, strain and modulus]]
	- [[#Types of Stress and Strain#Volumetric stress and strain|Volumetric stress and strain]]
	- [[#Types of Stress and Strain#Engineering strain vs True strain|Engineering strain vs True strain]]

Not completed sections:
- Mechanical behaviour
	- Strain hardening
		- Back to stress-strain graph, UTS and fracture strength
		- Comparison of yield strength
		- Comparison of UTS
	- Ductility
		- % elongation
		- % reduction of area at fracture (during necking)
		- Importance of ductility in material selection
		- Brittle vs Ductile fracture patterns
	- Toughness
	- Hooke's Law in materials
		- Hooke's Law in shear
		- Hooke's Law in bulk modulus
	- Elastic deformation
		- Poisson ratio definition
	- Plastic deformation (permanent, opposite of elastic deformation)
- Practical Design Considerations
	- Polymers and material selection
		- Basic idea of polymers
		- Stress-strain curve for different polymers
		- Glass transition $T_{g}$ and melting point $T_{m}$
	- Ashby's design rules
		- Materials index $M_{1}$ (important!!!)
		- Common list of valence electron numbers
- Misc stuff to know
	- AZ31
	- VESTA software

# Introduction to Material Science

## Classification of Materials

In general, there are 5 families of materials: Metals, Ceramics, Polymers, Natural Materials, and Composites.

![[Pasted image 20240122125645.png|450]]

![[Pasted image 20240122125709.png|450]]

**Note:** exams will test your knowledge on the types and examples of ceramics and polymers. Don't forget the difference between thermosets (e.g. PS) and thermoplastics (e.g. PLA) as they are very common. 

# Review of chemical concepts

> TODO: impact on deformability/elasticity

## Chemical Bonding

To understand structures and materials, we only need to consider the common things in an atom: proton, neutron and electrons.

### Bond Energy and Length

All bonding has an energy/length graph showing what's the energy state of a bond given a certain bond length (distance between 2 atoms). 

![[Pasted image 20240212004824.png|500]]
*(Credits: University of Wisconsin [CHEMISTRY 109 FALL 2021](https://wisc.pb.unizin.org/chem109fall2021ver02/))*

For example, in the graph above showing the energy/distance graph for 2 hydrogen atoms, at 74pm the lowest energy is recorded on the graph, meaning that it is nicely bonded. Pushing the atoms any closer or further increases this bond energy (for e.g., at 300pm the bond is broken, requiring an energy change of 436kJ/mol). 

*Reference: James Page 50/Section 2.5: The Secondary, or van der Waals, Bond*

Specifically for **secondary bonding**, the 12-6 or 6-12 potential describes the energy curve:
$$
E = \frac{K_{A}}{a^{6}} + \frac{K_{R}}{a^{12}}
$$
where:
- $E$ is bond energy
- $K_{A}$ is constant for attraction $-10.37\times 10^{-78} \pu{ J\cdot m^{6} }$
- $K_{R}$ is constant for repulsion $16.16\times 10^{-135} \pu{ J\cdot m^{12} }$
- $a$ is the bond length

To solve for equilibrium bond length (i.e. lowest part of the curve where the lowest bond energy is), simply find the location where $\frac{ \mathrm{d}E }{ \mathrm{d}a }=0$ (since the graph is flat at that region). As such, all you have to do is to solve for $a_{0}$ in:

$$
\left( \frac{ \mathrm{d}E }{ \mathrm{d}a } | _{a=a_{0}} \right) = 0 = \frac{6K_{A}}{{a_{0}}^{7}} - \frac{12K_{R}}{{a_{0}}^{13}}
$$

### Primary Bonds

#### Ionic bond

*Reference: James Page 29/Section 2.2: The ionic bond*

It is made through electron transfer creating a more stable electron configuration. Electron is being moved from one atom to another creating positive and negative ions, resulting in all the atoms in the bond having a full outer orbital shell. 
##### Coordination Number (CN)

This is the number of neighbouring ions that surround an ion/atom that allows it to be stable. 

![[Pasted image 20240211181613.png|500]]

In the picture above, you can see how a single ion with a given size can only have a maximum of 3 as its CN. You just can't fit 4 ions with one electron between them!

To calculate Coordination Number, you need to figure out the radius ratio, and compare it to the lookup table provided:
$$
\text{Radius Ratio} = \frac{r}{R} = \frac{\text{radius of smaller atom}}{\text{radius of larger atom}}
$$

![[Pasted image 20240211183544.png]]

You can obtain the full list of atomic and ionic radii in Appendix 2 of the textbook.

![[Pasted image 20240211154557.png|200]]

#### Covalent bond

Electrons are shared in a covalent bond between atoms, which leads us into the possibility of polymerisation. We will explore polymers in a later chapter.

![[Crystalline-structure-of-a-graphite-and-b-diamond.png|400]]

As valence electrons are shared between neighbouring atoms, they typically have higher melting temperatures and higher hardness. Notably, diamond has a microstructure of directional covalent bonding, and since diamond has a higher CN than graphite (4 vs 3) which makes it much harder than graphite. 

#### Metallic bond

In a metallic bond, the valence electrons are all "floating" around known as delocalised electrons. 

![[Pasted image 20240211233659.png|400]]
### Secondary Bonds

There's generally just 2 types of secondary bonds, Van der Waals bonding or Hydrogen bonding. 

![[Pasted image 20240211234028.png]]

Van der Waals bonds are held together by differing dipole charges, in which the distribution of electrons are altered. 

# Crystalline Structures

Most engineering materials has crystalline structures, which means that the atoms are arranged in regular and repeating patterns. There are a total of 7 crystal systems and 14 crystal lattices that we will see later. 

![[Pasted image 20240212010327.png]]

The fundamental unit of a crystalline structure is called a unit cell, which is the smallest unit that can describe the entire structure. It consists of 6 parameters, $abc$ for length and $\alpha \beta \gamma$ for angles between the axes. 

## Types of crystal structures

*Reference: James Page 59/Section 3.1: Seven Systems and Fourteen Lattices*

The 7 crystal systems are listed below (for the most part, we will be looking at cubic which has exactly the same side length $a$, and where $\gamma=90\degree$):

![[Pasted image 20240212010454.png]]

The 14 crystal lattices, also known as Bravais lattices, are listed below (most elemental metals at room temperatures will be BCC, FCC or HCP. Midterms will not test HCP):

![[Pasted image 20240212010522.png]]

## Miller Indices

*Reference: James Page 81/Section 3.6: Lattice Positions, Directions, and Planes*

Miller indices are used to represent positions, directions and planes within lattices (usually within a single unit cell). When a direction or plane is in the "Family" notation, it means that these directions/planes are structurally equivalent. A quick example is that $<111>$ is equivalent to $[\bar{1}11], [1\bar{1}1],[11\bar{1}],\dots$.

| Classification | Notations | Examples | Family |
| ---- | ---- | ---- | ---- |
| Lattice positions | $x\ y\ z$ | $2 2 1$ | N/A |
| Directions | $[hkl]$ | $[1\bar{1}0]$ | $<hkl>$ |
| Planes | $(hkl)$ | $(001)$ | $\{ hkl \}$ |
### Positional indices

![[Pasted image 20240212012333.png|600]]

The above diagram shows us how to read Miller indices for **positions** in a lattice. In positional indices, fractions are allowed.

### Directional indices

![[Pasted image 20240212140521.png|600]]

The above diagram shows us how to read Miller indices for **directions**. In the right diagram, the family of figures $<111>$ encompasses all the directions depicted by the arrows. In constructing direction indices for a single unit cell, take note that fractions are **not** allowed because the arrow will eventually intersect at a point with a whole number (for e.g. the direction $[112]$, which only passes through the point $\frac{1}{2} \frac{1}{2} 1$ in its own unit cell. It needs to be multiplied to reduce the fraction to a whole number).

Directions also play an important role in determining linear density later on. Linear density of the number of atoms intersected by a direction vector, over the length of the direction vector. You can see it in action with an FCC structure and a direction of $[110]$ below.  

![[main-qimg-79ac74b600f397a20d525638df959814 copy.png|400]]

Linear density is an important concept when talking about direction-dependent elasticity characteristics, that we will encounter later.

### Planar indices

![[Pasted image 20240212014032.png|600]]

The above diagram shows us how to read Miller indices for **planes**. 

![[Pasted image 20240212142024.png]]

Planar indices also have families. In the diagram above, we see the $\{ 100 \}$ family consisting of all 6 faces of the cube. 

To represent a plane, you have to do the following steps:
1. **Find the intercepts**. In the top example, the intercepts are $\frac{1}{2},1,\infty$. Note that $\infty$ intercepts means that the plane does not intercept that axis at all
2. **Find the reciprocals**. $\frac{1}{1/2}, \frac{1}{1}, \frac{1}{\infty}$
3. **Resolve the fractions and quote the result**. $(210)$

> [!WARNING] Do not use the wrong format!
> Miller indices are very particular about the format. While you can use commas in intermediate steps to show that the numbers are different, do not write results in an improper format. Some examples for wrong formats include:
> - $(1,1,1)$ no commas allowed
> - $(1-11)$ negative sign not written as a bar
> - $211$ failure to quote a plane, meaning that you effectively wrote a position, not a plane

![[Pasted image 20240212135858.png]]
*(Credits: Fig 4.3.5, Elliot)*

In addition, we must also be careful when constructing a planar index when the plane intersects the origin. You have to relocate/redefine the origin to another point in the unit cell to avoid the plane intersecting the origin, similar to what's depicted in the figure above. 

Planar indices assist us in finding out the planar density and packing fraction, which are defined by:
$$
\begin{align}
\text{Planar density}  & = \frac{\text{atoms per face}}{\text{area of face}} \\ \\
\text{Packing fraction}  & = \frac{\text{area of atoms per face}}{\text{area of face}}
\end{align}
$$

![[Pasted image 20240212142657.png|400]]

Essentially you take the "slice" of the plane and see how many atoms/area of atoms there are to obtain the numerator. In the above diagram we can see that taking the $(010)$ vs $(020)$ planes result in very different planar densities. **Planar density is directly associated with the hardness of material on that plane**. 

## Crystal Defects

*Reference: James Page 104/Chapter 4: Crystal Defects and Noncrystalline Structure—Imperfection*

Nothing is perfect in this world, and our crystalline structures are no different. This part will go over common crystal defects. 

### Solid solutions and hardening

![[Pasted image 20240212150008.png|400]]

All of us are probably familiar with the concept of liquid solutions (e.g. vodka is 40% ethanol and 60% water ( ͡o ͜ʖ ͡o) ), in which mixing of the 2 molecules occurs on a molecular scale (see left diagram). Solids can also be solutions too! In the right diagram, we can see a solid solution of nickel in copper. Copper is the solvent, and nickel is the solute in this case.

Notice that in the Cu-Ni case we see, the atomic radii of the two atoms are quite similar, and they swap out one another's positions in a "substitutional solid solution". When the atomic sizes differ too much, different solutions may exist such as interstitial solutions, where the much smaller atom squeezes between the larger ones. 

**Solid solution hardening** is when atoms of different sizes is introduced into a crystal lattice, hindering dislocation movements and therefore increasing material hardness. 

### Point Defects

*Reference: Elliot Page 76/Section 4.5: Crystalline Defects*

Point defect is the simplest type of defect that occurs in points within the crystal structure. 

![[Pasted image 20240212150656.png]]

There are 3 types of point defects:
(a) Vacancy: where one atom is missing. This results in volume reduction
(b) Substitutional impurity: where one local atom is substituted for a foreign atom
(c) Interstitial impurity: where one foreign atom squeezes between the existing atoms. This results in volume expansion. 

Point defects will eventually affect different moduli due to valence electron count and volume changes. 

### Interstitial Solutions

We've seen how there can be interstitial point defects, which is linked to the concept of interstitial solutions, where a smaller atom embeds itself in the structure of a crystal lattice of a bigger atom. 

![[Pasted image 20240213001353.png]]

In Figure 4.4, you can see a interstitial solid solution of a carbon atom embedded in the lattice of iron atoms. This happens when substituting a much smaller atom in place of an existing larger atom is energetically unstable, and as such it chooses to be more stable in between atoms. 

The solubility of one atom in another atom's crystal structure is determined by how oversized it is. Too large and the solubility goes down. 

In the example above of carbon in iron, we can calculate the ratio between the optimal interstitial radius vs the actual radius of the carbon atom. If the ratio >1, that means it's too large to fit and therefore results in **low solubility**. 

### Linear defects

Linear defect, aka dislocations, follows a path throughout the crystal structure (like a crack on the wall). Line defects occur when a row of atoms do not line up correctly within a crystal structure. 

This type of defects forms the foundation of slip systems, and will be further discussed with plasticity and fractures in week 10 and 11. 

![[Pasted image 20240212151054.png]]

In figure 4.10 we see an edge dislocation, where an entire row of atoms is added on top. 

![[Pasted image 20240212151411.png]]

In figures 4.12 and 4.13, we see examples of screw dislocation and mixed dislocation (both edge and screw dislocation).

For now we don't need to know too much about them other than they exist :)

### Planar defects

Planar defects are boundaries between a near-perfect crystalline region and some other part of the material. For our course, we will mainly be looking at **grain boundary** planar defects, where 2 single crystals or grains meet. 

The vast majority of engineering materials outside of electronics or aerospace are polycrystalline, which is where multiple single crystals adhere together with boundaries at their interfaces. 

![[Pasted image 20240212163209.png|183]]                        ![[Pasted image 20240212154838.png|230]]

Figure 4.18 shows us the simplest possible grain boundary, called a tilt boundary because as the name suggests, the 2 crystalline regions are offset to one another by a certain angle. 

Figure 4.17 is what planar defects look like in real life, when you see the grain structure in a metal. 

### Shape memory effect in NiTi

![[Pasted image 20240213110721.png|350]]
*(Credit: [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:NiTi_structure_transformation.jpg))*

NiTi alloy also known as nitinol is a shape memory alloy, which takes up 2 primary states: martensite or austenite. 


# Phase Diagrams

Phase diagrams in material science are very similar to the phase diagrams we might have already learned in secondary school/JC, such as the water phase diagram under different temperatures and pressures:

![[Pasted image 20240213110958.png|400]]

A phase in the diagram above refers to either gaseous, liquid or solid, each with its own different arrangement of atoms. 

Just like the water example we've seen above, phase diagrams can also represent different phases of matter for a given material. 

![[Pasted image 20240213111124.png|400]]

In Figure 9.4, we see a diagram for pure iron in liquid or gas state, and in addition to liquid/gas we also see $\alpha,\gamma,\delta$ phases. These Greek-lettered phases are specifically to indicate the microstructure of the iron itself and other properties.
- $\alpha$: ferrite iron, has a bcc crystal structure
- $\gamma$: austenite, has an fcc crystal structure
- $\delta$ delta-iron, changes back into bcc crystal structure
For more information see [Allotropes of iron](https://en.wikipedia.org/wiki/Allotropes_of_iron)

Now, the phase diagrams that we are really interested in are **binary diagrams**, or diagrams that show a mixture of 2 elements on the x-axis, and temperature on the y-axis. As you can see below, binary diagrams kinda looks like a pikachu.

![[Pasted image 20240213112620.png|400]]![[pikachu.png|300]]

Remember, phase diagrams differ wildly from binary system to system (i.e. different solutions of elements). In each part of the phase diagram, the structures could look completely different, and hence that's why phase diagrams are referred to as a "map", because by reading the two axes of the diagram, you can find out exactly what the material's microstructure looks like, which also helps you to determine the material properties. 


> [!WARNING] Not all phase diagrams look like this!
> ![[Pasted image 20240213112011.png|400]]
> The pikachu-looking phase diagrams describe what's known as a "limited solid solution diagram", meaning that the diagram does not take pressure into account, and dedicates majority of the diagram to the solid state. The uppermost quadrant labelled L is entirely in the liquid state. 
> 
> There are many other types of phase diagrams, but for this course, we will only look at limited solid solution diagrams.

## Example of an Mg-Al system

![[Pasted image 20240213142500.png|500]]
*(Credit: [Essential Magnesium Alloys Binary Phase Diagrams and Their Thermochemical Data](https://doi.org/10.1155/2014%2F704283)*)

In the original lesson slides we are introduced to the Magnesium-Aluminium binary system. On the extreme left and right side are 100% Aluminium (Fcc-Al) and 100% Magnesium (Mg-Hcp) respectively, also known as the $\alpha$-phase for both elements. On the very top in the liquid state is the $\gamma$-phase. The bottom left and bottom right quadrants consist of a mixture of $\gamma$-phase structures and the original Fcc-Aluminium or Hcp-Magnesium. 

Notably, the $\gamma$-phase is harder than $\alpha$-phase, due to its crystalline structure that has all those defects, compared to an $\alpha$-phase which is a pure element. 

![[Pasted image 20240213150600.png|500]]

Under a microscope, we can see the grain boundaries and different phases of material existing within one another. (Note that AZ31 is 3% Al, 96% Mg, while AZ91 is 10% Al, 89% Mg, with the rest being other metals).

# Mechanical behaviour

*Reference: James Page 152/Section 6: Mechanical Behaviour*

In this chapter we will look at how these microscopic features translate into macroscopic material properties. 

## Definition of Stress and Strain

Most commonly, when we want to found out if some material is "strong", we subject it to a tensile test which is a fancy way of saying "stretching the sh\*t out of it". 

Engineering stress, which is unfortunately not defined by how much stress an average engineering student experiences but rather:
$$
\sigma = \frac{P}{A_{0}}
$$
where:
- $P$ is the load on the sample ($\pu{ N}$)
- $A_{0}$ is the area of the cross-section of the sample under test ($\pu{ m^{2}}$)
- $\sigma$ is stress ($\pu{N/m^{2}}$)


Engineering strain is a ratio of how much a material deforms under load, and is defined as:

$$
\varepsilon = \frac{\Delta l}{l_{0}}
$$
where:
- $\Delta l$ is the amount of length changed
- $l_{0}$ is the original length of the sample

## Stress-Strain Relationship Curve

![[Pasted image 20240213171620.png|500]]
*(Credit: [BYJUS](https://byjus.com/physics/stress-and-strain/))*

> [!NOTE] Recall Hooke's Law
> Hooke's Law simply states that certain materials change their lengths proportional to the amount of force they receive, just like an ideal spring. 

When we stretch a given sample, we can graph the characteristics of how much stress is being loaded vs how much the load stretches out (i.e. strain). There are several discrete regions that have their own characteristics:

- **From 0 to A**: This is where we measure **Young's Modulus** by calculating the gradient of this region. This is also the region where the material respects Hooke's Law and "behaves like a spring" because it can spring back to point 0 when the stress is unloaded.
- **Point B**: The **elastic limit** is reached, which is the maximum point in the graph in which the material will still undergo elastic deformation. Go beyond this point and the material only plastically deforms.
- **From B to C**: By now, the material will only undergo plastic deformation, meaning that it will not spring back to point 0. Notice that at point C (the lower-yield point) the maximum length it will spring back is at the same strain level as point B. **Strain hardening** also starts to occur, where more dislocations form, which further resists plastic deformation. We will see this later in the concept of "Cold working".
- **Point D**: The **ultimate tensile strength** $\sigma_{UTS}$ has been reached. This is the maximum stress possible on this material without breaking. 
- **From D to E**: **Necking** starts to occur for certain materials at this point. Necking is when the material starts to become thinner and thinner right before it fractures.
- **Point E**: The **fracture strain** at this point represented by $\varepsilon_{F}$ is the maximum possible strain before the material breaks completely.

The **area under graph** can also derive another characteristic of this material: **Toughness**. Toughness is the energy required to break the material. 

> [!WARNING] Confused about Proportional Limit vs Elastic Limit?
> **Proportional limit** at point A is when the material stops following Hooke's Law (i.e. it can deform proportionally to the force given to it). 
> **Elastic limit** at point B is when the material stops being elastic and will start to deform plastically. 
> 
> The slides don't really differentiate between proportional and elastic limit because it is hard to differentiate between the point at which it no longer follows Hooke's Law *(Reference: James Chapter 6 p. 154)*. 
> 
>  Throughout this text we will use the term "proportional limit" and not "elastic limit" to refer to the end of linearity in the graph.
^9326f0

> [!WARNING] Not all materials have this shape of curve!
> The curve shown above is one that only covers the most common shapes. Common stress-strain graphs for metal, plastics and ceramics are shown below:
> 
> ![[Pasted image 20240213180916.png|500]]

## Data from Tensile Testing

Tensile testing gives us the graph that we see above, and many other valuable data we can derive from that graph:

### Young's Modulus

![[Pasted image 20240213190731.png|300]]

We can obtain Young's modulus ($E$) by either finding out the slope of the elastic region, or by determining the bond stiffness and length:
$$
E=\frac{\sigma}{\varepsilon_{n}} = \frac{S_{0}}{r_{0}}
$$
where:
- $\sigma$ is the stress at the proportional limit (see [[#^9326f0]] for definition)
- $\varepsilon_{n}$ is the strain at the proportional limit
- $S_{0}$ is bond stiffness (i.e. bond stiffness goes up, $E$ goes up)
- $r_{0}$ is bond length (i.e. bond length goes down, $E$ goes up)
- $E$ is Young's modulus
#### Bond stiffness

Bond stiffness plays a central role in determining $E$, and is defined by the equation
$$
F = S_{0}
(r-r_{0})$$
where:
- $F$ is the force to separate 2 atoms by distance $r$
- $r$ is the new distance between 2 atoms
- $r_{0}$ is the original distance between 2 atoms
- $S_{0}$ is the bond stiffness

Re-examining the $E$ equation above, we realise that Young's modulus is really just the bond stiffness normalised (averaged) by the length of the bond $r_{0}$. 

#### Valence electron density and $E$

Young's modulus is influenced by many factors, one of which is valence electron density. As a result, covalently bonded structures usually have a higher Young's modulus compared to ionically bonded ones. 

![[Pasted image 20240213220135.png|500]]
*(Credit: Ashby Page 85/Section 6.2: Moduli of Crystals)*

> [!NOTE] Confusing proportionality
> In the slides, we also see a mention that Young's modulus is proportional to the square of charge over the (atomic volume)$^{4/3}$. The reason why this exists is due to the definition of $S_{0}$ or bond stiffness, where $q$ or charge is squared in the numerator:
> $$S_{0} = \frac{\alpha q^{2}}{4\pi\varepsilon_{0}r_{0}^{3}}$$
> As such, the slides state that:
> $$ E \propto \frac{q^{2}}{V^{4/3}} $$
> The same concept can be applied to other moduli as well, such as bulk modulus as we will see later.

### Yield Strength

![[Pasted image 20240213222157.png|500]]

Yield strength $\sigma_{y}$ is the stress value $\sigma$ (y-axis) at the a point created by the intersection of a straight line that's 0.2% (0.002) away from the origin with the stress-strain curve (see Figure 6.6 circle 2 for the yield strength point in this graph).

Why 0.2%? Because yield strength is defined usually as the **stress necessary to generate a small amount of permanent deformation (of 0.2%)**. 

### Ultimate Tensile Strength

![[Pasted image 20240213171620.png|250]]

The highest point of stress on a stress-strain curve is the Ultimate Tensile Strength $\sigma_{UTS}$, the absolute maximum in which a material can withstand without breaking. See point D on the above diagram for the ultimate tensile strength. 

### Total % elongation / Ductility

![[Pasted image 20240213224122.png]]
*(Credits: [idk where's this lol somewhere in IL,USA](https://nanohub.org/resources/6054/download/ch07_stress-strain.pdf))*

Ductility is a measure of how much a material can keep getting plastically deformed before fracturing. There are 2 measures of ductility that can be computed from a tensile test, percent elongation and percent reduction of area:
$$
\% \text{ elongation} = \frac{l_{f}-l_{0}}{l_{0}} \times 100
$$
where: 
- $l_{f}$ is the final length of sample
- $l_{0}$ is the initial length of sample
$$
\% \text{AR} = \frac{A_{0}-A_{f}}{A_{0}} \times  100
$$
where: 
- $A_{f}$ is the final cross-section area of the sample (usually when necking occurs)
- $A_{0}$ is the initial cross-section area of the sample
 
## Types of Stress and Strain

Just like how our profs put us through stress, we are going to put some materials through stress as well. These are the classifications of stress in materials.

### Normal stress

Normal stress is simply stress caused by pulling a piece of material apart (tension) or pushing it together (compression). It is when the force is normal (90 degrees) to the cross sectional area it's working on.


### Shear stress, strain and modulus

Shear stress is when the stress is parallel with the plane it's acting upon. A common example is when stuff slides apart. 

![[Pasted image 20240213225650.png|400]]![[Pasted image 20240213225927.png|300]]
*(Credit: [BYJUS](https://byjus.com/physics/shearing-stress/))*

Shear stress is defined by 
$$
\tau = \frac{P_{s}}{A_{s}}
$$
where:
- $P_{s}$ is the load on the sample ($\pu{ N}$)
- $A_{s}$ is the area of the sample parallel ($\pu{ m^{2}}$)

Shear strain is a bit different as it is based on an angular displacement:
$$
\gamma = \tan \alpha = \frac{\Delta y}{z_{0}}
$$
where:
- $\alpha$ is the angle displaced; or alternatively
- $\Delta y$ is the displacement along the y-axis
- $z_{0}$ is the original z-height of the item

Shear modulus, aka the modulus of rigidity is simply defined as a ratio of the stress over strain (just like how Young's modulus is also $\frac{\sigma}{\varepsilon} = \frac{\text{stress}}{\text{strain}}$!):
$$
G = \frac{\tau}{\gamma}
$$

> TODO: relate this to Poisson ratio
### Volumetric stress and strain

> TODO

### Engineering strain vs True strain

*Reference: [ANSYS Mechanical Strain in Deformation Analysis – Lesson 3](https://courses.ansys.com/wp-content/uploads/2020/05/Lesson-3-Engineering-Strain-and-True-Strain.pdf)*

Recall that strain is just a ratio of displacement, i.e. how much something was displaced relative to its original dimension (be it length, angle or volume). 

There are two types of strain, **engineering strain** and **true strain**. 

![[Pasted image 20240213231425.png|500]]

Engineering strain is the "lazier" approach by comparing the initial length to the final length to determine deformation (simple algebra). However for the majority of applications engineering strain would suffice. 
$$
\varepsilon_{E} = \frac{\Delta L}{L_{0}}
$$
where:
- $\Delta L$ is the change in length of sample
- $L_{0}$ is the initial length of sample

![[Pasted image 20240213231440.png|500]]

True strain measures the actual length at every instance of a load stress to determine deformation (thus requiring integration). True strain $\varepsilon_{T}$ is usually modelled as a logarithmic function:
$$
\varepsilon_{T} = \ln\left( 1+ \frac{\Delta L}{L_{0}} \right) = \ln\left( \frac{L_{0} + \Delta L}{L_{0}} \right) = \ln\left( \frac{\text{Final length}}{\text{Initial length}} \right)
$$

With larger and larger deformations, we can see that the true strain and engineering strain graphs start to diverge. 

![[Pasted image 20240213231858.png]]


























