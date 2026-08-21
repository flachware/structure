# **On the Structure of Type**<br>An Essay Towards a Formal Definition<br>*by Johannes Krtek*

A glyph is a word from another alphabet. More specifically, a glyph is a word from a *spatial alphabet*. Its symbols represent directions in the space we inhabit.

First, we need space. Not just any space: its directions must be perceptually discriminable with ease. We therefore begin with the smallest discrete spatial unit: a single voxel.

Figure: 1 voxel

A single voxel represents merely a single state; there is no way to derive direction from it. We therefore add its neighbours, creating the smallest symmetric 3D space grid possible.

Figure: space grid

The resulting <math xmlns="http://www.w3.org/1998/Math/MathML" display="inline"> <mo>(</mo> <mn>3</mn> <mo>×</mo> <mn>3</mn> <mo>×</mo> <mn>3</mn> <mo>)</mo> </math> grid contains 27 states. With the central voxel as the reference state, the remaining 26 states define 26 discrete directions — coincidentally matching the 26 letters of the alphabet. This is our *spatial alphabet* <math xmlns="http://www.w3.org/1998/Math/MathML" display="inline"><mi>𝒜</mi></math>:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block"> <mi>𝒜</mi> <mo>=</mo> <msup> <mrow> <mo>{</mo> <mo>−</mo><mn>1</mn><mo>,</mo><mn>0</mn><mo>,</mo><mn>1</mn> <mo>}</mo> </mrow> <mn>3</mn> </msup> <mo>∖</mo> <mo>{</mo> <mo>(</mo><mn>0</mn><mo>,</mo><mn>0</mn><mo>,</mo><mn>0</mn><mo>)</mo> <mo>}</mo> </math>

Figure: All voxels

Hence, a *spatial word* is a sequence of spatial states, represented by voxels:

Figure: voxel word

These states can be expressed as vectors over the alphabet <math xmlns="http://www.w3.org/1998/Math/MathML" display="inline"><mi>𝒜</mi></math>, yielding a vector sequence:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mi>W</mi>
  <mo>=</mo>
  <mo>(</mo>
  <mo>(</mo><mo>−</mo><mn>1</mn><mo>,</mo><mo>−</mo><mn>1</mn><mo>,</mo><mn>0</mn><mo>)</mo>
  <mo>,</mo>
  <mo>(</mo><mn>1</mn><mo>,</mo><mo>−</mo><mn>1</mn><mo>,</mo><mn>0</mn><mo>)</mo>
  <mo>,</mo>
  <mo>(</mo><mn>1</mn><mo>,</mo><mn>1</mn><mo>,</mo><mn>0</mn><mo>)</mo>
  <mo>,</mo>
  <mo>(</mo><mo>−</mo><mn>1</mn><mo>,</mo><mn>1</mn><mo>,</mo><mn>0</mn><mo>)</mo>
  <mo>)</mo>
</math>

Figure: vector word

Since the symbols of our *spatial alphabet* are vectors, we can also represent them geometrically:

Figure: vector diagram


<br><br><br><br><br><br><br><br><br><br><br><br><br><br>

Together, these 26 directions form the *spatial alphabet* <math xmlns="http://www.w3.org/1998/Math/MathML"><mi>𝒜</mi></math>:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mi>𝒜</mi>
  <mo>=</mo>
  <mo>{</mo>
  <mrow>
    <mi>a</mi><msub><mi>𝒗</mi><mi>x</mi></msub>
    <mo>+</mo>
    <mi>b</mi><msub><mi>𝒗</mi><mi>y</mi></msub>
    <mo>+</mo>
    <mi>c</mi><msub><mi>𝒗</mi><mi>z</mi></msub>
  </mrow>
  <mo>|</mo>
  <mi>a</mi><mo>,</mo><mi>b</mi><mo>,</mo><mi>c</mi>
  <mo>∈</mo>
  <mo>{</mo><mo>−</mo><mn>1</mn><mo>,</mo><mn>0</mn><mo>,</mo><mn>1</mn><mo>}</mo>
  <mo>,</mo>
  <mo>(</mo><mi>a</mi><mo>,</mo><mi>b</mi><mo>,</mo><mi>c</mi><mo>)</mo>
  <mo>≠</mo>
  <mo>(</mo><mn>0</mn><mo>,</mo><mn>0</mn><mo>,</mo><mn>0</mn><mo>)</mo>
  <mo>}</mo>
</math>

Hence a *spatial word* is represented as a sequence of vectors over the Alphabet <math xmlns="http://www.w3.org/1998/Math/MathML" display="inline"><mi>𝒜</mi></math>:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mi>W</mi>
  <mo>=</mo>
  <mo>(</mo>
  <mo>(</mo><mo>−</mo><mn>1</mn><mo>,</mo><mo>−</mo><mn>1</mn><mo>,</mo><mn>0</mn><mo>)</mo>
  <mo>,</mo>
  <mo>(</mo><mn>1</mn><mo>,</mo><mo>−</mo><mn>1</mn><mo>,</mo><mn>0</mn><mo>)</mo>
  <mo>,</mo>
  <mo>(</mo><mn>1</mn><mo>,</mo><mn>1</mn><mo>,</mo><mn>0</mn><mo>)</mo>
  <mo>,</mo>
  <mo>(</mo><mo>−</mo><mn>1</mn><mo>,</mo><mn>1</mn><mo>,</mo><mn>0</mn><mo>)</mo>
  <mo>)</mo>
</math>

Figure: left down, right down, right up, left up

<br><br><br><br><br><br><br>

We may take <math xmlns="http://www.w3.org/1998/Math/MathML" display="inline"><msub><mi>𝒆</mi><mi>x</mi></msub></math>, <math xmlns="http://www.w3.org/1998/Math/MathML" display="inline"><msub><mi>𝒆</mi><mi>y</mi></msub></math>, and <math xmlns="http://www.w3.org/1998/Math/MathML" display="inline"><msub><mi>𝒆</mi><mi>z</mi></msub></math> as the unit vectors along the three coordinate axes of <math xmlns="http://www.w3.org/1998/Math/MathML" display="inline"><msup><mi>ℝ</mi><mn>3</mn></msup></math>. The six fundamental directions then constitute our spatial alphabet:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mi>𝒜</mi>
  <mo>=</mo>
  <mo>{</mo>
  <msub><mi>𝒆</mi><mi>x</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <msub><mi>𝒆</mi><mi>y</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <msub><mi>𝒆</mi><mi>z</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <mo lspace="0.03em" rspace="0.03em">−</mo>
  <msub><mi>𝒆</mi><mi>x</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <mo lspace="0.03em" rspace="0.03em">−</mo>
  <msub><mi>𝒆</mi><mi>y</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <mo lspace="0.03em" rspace="0.03em">−</mo>
  <msub><mi>𝒆</mi><mi>z</mi></msub>
  <mo>}</mo>
</math>

Hence a spatial word is represented as a sequence of vectors over the Alphabet <math xmlns="http://www.w3.org/1998/Math/MathML" display="inline"><mi>𝒜</mi></math>:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mi>W</mi>
  <mo>=</mo>
  <mo>(</mo>
  <mo lspace="0.03em" rspace="0.03em">−</mo><msub><mi>𝒆</mi><mi>x</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <mo lspace="0.03em" rspace="0.03em">−</mo><msub><mi>𝒆</mi><mi>y</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <mo lspace="0.03em" rspace="0.03em">−</mo><msub><mi>𝒆</mi><mi>y</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <msub><mi>𝒆</mi><mi>x</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <msub><mi>𝒆</mi><mi>x</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <msub><mi>𝒆</mi><mi>y</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <msub><mi>𝒆</mi><mi>y</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <mo lspace="0.03em" rspace="0.03em">−</mo><msub><mi>𝒆</mi><mi>x</mi></msub>
  <mo>)</mo>
</math>

<figure>
  <svg width="1920" height="1080" viewBox="0 0 1920 1080">
    <rect x="calc(50% - 250px)" y="calc(50% - 250px)" width="500" height="500" fill="none" stroke-width="4" stroke="var(--primary)"/>
  </svg>
  <div class="container-fluid">
    <figcaption>Figure: the spatial word for the letter o.</figcaption>
  </div>
</figure>

As the symbols of the spatial alphabet are vectors, the word admits algebraic operations: its constituent vectors may be summed to obtain its effective displacement. Just as Cartesian geometry rendered spatial relations calculable through their representation by coordinates, the vector alphabet makes the structure of the spatial word amenable to calculation.

Since a spatial word has no temporal dimension, serial vectors may be interpreted as components of a spatial change rather than as a temporal sequence. Adjacent orthogonal vectors can therefore be combined by vector addition into single resultant vectors while preserving the spatial extent of the word.

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mtable columnalign="left" rowspacing="1.2em">
    <mtr>
      <mtd>
        <mo>(</mo>
        <mo lspace="0.03em" rspace="0.03em">−</mo><msub><mi>𝒆</mi><mi>x</mi></msub>
        <mo lspace="0em" rspace="0.3em">,</mo>
        <mo lspace="0.03em" rspace="0.03em">−</mo><msub><mi>𝒆</mi><mi>y</mi></msub>
        <mo>)</mo>
        <mo>→</mo>
        <mo lspace="0.03em" rspace="0.03em">−</mo><msub><mi>𝒆</mi><mi>x</mi></msub>
        <mo>−</mo><msub><mi>𝒆</mi><mi>y</mi></msub>
      </mtd>
    </mtr>
    <mtr>
      <mtd>
        <mo>(</mo>
        <msub><mi>𝒆</mi><mi>x</mi></msub>
        <mo lspace="0em" rspace="0.3em">,</mo>
        <msub><mi>𝒆</mi><mi>y</mi></msub>
        <mo>)</mo>
        <mo>→</mo>
        <msub><mi>𝒆</mi><mi>x</mi></msub>
        <mo>+</mo><msub><mi>𝒆</mi><mi>y</mi></msub>
      </mtd>
    </mtr>
    <mtr>
      <mtd>
        <mo>(</mo>
        <msub><mi>𝒆</mi><mi>y</mi></msub>
        <mo lspace="0em" rspace="0.3em">,</mo>
        <mo lspace="0.03em" rspace="0.03em">−</mo><msub><mi>𝒆</mi><mi>x</mi></msub>
        <mo>)</mo>
        <mo>→</mo>
        <msub><mi>𝒆</mi><mi>y</mi></msub>
        <mo>−</mo><msub><mi>𝒆</mi><mi>x</mi></msub>
      </mtd>
    </mtr>
  </mtable>
</math>

This yields a representation with two-dimensional vector symbols:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mi>W′</mi>
  <mo>=</mo>
  <mo>(</mo>
  <mo lspace="0.03em" rspace="0.03em">−</mo><msub><mi>𝒆</mi><mi>x</mi></msub>
  <mo>−</mo>
  <msub><mi>𝒆</mi><mi>y</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <mo lspace="0.03em" rspace="0.03em">−</mo><msub><mi>𝒆</mi><mi>y</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <msub><mi>𝒆</mi><mi>x</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <msub><mi>𝒆</mi><mi>x</mi></msub>
  <mo>+</mo>
  <msub><mi>𝒆</mi><mi>y</mi></msub>
  <mo lspace="0em" rspace="0.3em">,</mo>
  <msub><mi>𝒆</mi><mi>y</mi></msub>
  <mo>−</mo>
  <msub><mi>𝒆</mi><mi>x</mi></msub>
  <mo>)</mo>
</math>

Thus,
  <math xmlns="http://www.w3.org/1998/Math/MathML">
    <mi>W</mi>
    <mo>∼</mo>
    <mi>W′</mi>
  </math>
  are equivalent representations of the same spatial word.

Figure: the collapsed spatial word for the letter o

**A glyph is a spatial graph. As a symbol, the graph becomes a spatial signal, a carrier of symbolic information.**

<br><br><br><br><br><br><br>

To make explicit the structure of the spatial word, we may translate it into mathematical symbols. The spatial word is thereby represented as the relation <math xmlns="http://www.w3.org/1998/Math/MathML"><mi>R</mi></math> between points:

<math display="block" xmlns="http://www.w3.org/1998/Math/MathML">
  <mi>R</mi>
  <mo>=</mo>
  <mo stretchy="true">{</mo>
  <mrow>
    <mo stretchy="true">{</mo><msub><mi>P</mi><mn>1</mn></msub><mo>,</mo><msub><mi>P</mi><mn>2</mn></msub><mo stretchy="true">}</mo>
    <mo>,</mo>
    <mo stretchy="true">{</mo><msub><mi>P</mi><mn>2</mn></msub><mo>,</mo><msub><mi>P</mi><mn>3</mn></msub><mo stretchy="true">}</mo>
    <mo>,</mo>
    <mo stretchy="true">{</mo><msub><mi>P</mi><mn>3</mn></msub><mo>,</mo><msub><mi>P</mi><mn>4</mn></msub><mo stretchy="true">}</mo>
    <mo>,</mo>
    <mo stretchy="true">{</mo><msub><mi>P</mi><mn>4</mn></msub><mo>,</mo><msub><mi>P</mi><mn>1</mn></msub><mo stretchy="true">}</mo>
  </mrow>
  <mo stretchy="true">}</mo>
</math>

The mathematical description has the advantage of allowing us to formulate the relation between the symbols more precisely. While a word necessarily presents its symbols in sequence, the mathematical expression may represent their undirected relation.

Graph of points

Formulas

Figure: spatial graph

This spatial configuration is conventionally mapped to a specific grapheme and serves as its code. Not yet a complete graph or glyph, it constitutes its discrete identity – its fundamental information. Hence we may call it a *protograph*: the missing link between the grapheme <o> and the graph o.

Figure: grapheme – protograph – graph
