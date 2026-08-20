# **On the Structure of Type**<br>An Essay Towards a Formal Definition<br>*by Johannes Krtek*

A glyph is a word from another alphabet. More specifically, a glyph is a word from a *spatial alphabet*. Its six symbols are the fundamental directions of the space we inhabit.

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

Adjacent orthogonal vectors may be combined by vector addition, collapsing serial vectors into single resultant vectors.

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