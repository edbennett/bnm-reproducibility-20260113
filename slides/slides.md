# History

-

[![Photograph of statues of Newton and Leibniz](./images/newton_leibniz.jpg) <!-- .element: width="1000px" -->](https://commons.wikimedia.org/wiki/File:Statues_of_Isaac_Newton_and_Gottfried_Leibniz.jpg)

Notes:
Two of the finest scientists of the 17th century.
Both claimed to have invented calculus.
Likely that they both did, independently.
But neither claim could be proven
because the culture was to be secretive about your work
so you could make money by teaching it to those who wanted to learn.

-

![Photograph of the Royal Society's premises in Crane Court](./images/rs.jpg) <!-- .element: width="700px" -->

Notes:
Around the same time,
the Royal Society gets going.
Motto: "Nullius in Verba" - don't take anyone's word for it.
Starts the first scientific journal,
and promotes the philosophy that for your work to be recognised,
you must publish it,
in such a way that anyone can reproduce and understand it.

-

Process $\rightarrow$ Data $\rightarrow$ Analysis $\rightarrow$ Results

Notes:
The form of a paper was supposed to be this:
you explain what you did,
show what data that gave you,
show what you did to the data,
and then present the results of that process.
Simple,
logical,
and in principle anyone skilled in the art could follow it to reproduce you work.

-

![Photograph of a supercomputer](./images/supercomputer.jpg) <!-- .element: width="1200px" -->

Notes:
This was pretty successful for a few hundred years,
creating science as we know it.
Then in the twentieth century,
we taught sand how to think and gave it anxiety.
Great:
we now have (in principle) fully deterministic machines,
so we can share the exact set of steps,
and they can be reproduced precisely,
without the possibility of human error.

-

![Screen shot of a lot of code in very small font, filling the screen](./images/lots_of_code.png) <!-- .element: width="1800px" -->

Notes:
Unfortunately,
the length of instructions is longer than a typical paper,
even before you include the code of others that you're building on top of.

-

Process $\rightarrow$ ⬛ $\rightarrow$ 🪄 $\rightarrow$ ✨Results✨

Notes:
This,
and some early missteps like
"treating the computer like a piece of lab equipment",
meant that adopting computers actually reduce reproducibility
rather than improved it.

-

_An article about computational science in a scientific publication is **not** the scholarship itself, it is merely **advertising** of the scholarship. The actual scholarship is the complete software development environment and the complete set of instructions which generated the figures._

&mdash;[attributed to Jon Claerbout, around 1995](https://statweb.stanford.edu/~wavelab/Wavelab_850/wavelab.pdf)

Notes:
"Claerbout" rhymes with "share shout".
Returning to where we would like to be:
many people view papers as the ultimate goal.
But if they don't enable reproducibility,
then it is the supporting work
that forms the actual research.

-

![Graph showing the exponential growth in publications from 1650 to 2012](./images/publications.png) <!-- .element: width="800px" -->

[Bornmann and  Mutz, 2015, 10.1002/asi.23329](https://doi.org/10.1002/asi.23329)

Notes:
The success of the scientific method has also led to
an exponential growth in the number of publications over the centuries,
particularly in the last hundred years.

-

![Screen shot of the access charges for the article linked on the previous slide (&dollar;49 for a PDF)](./images/access_charges.png) <!-- .element: width="700px" -->

Notes:
The cost of gaining access to these publications has risen even more rapidly.

---

# Definitions

-

## Reproducibility

<span class="fragment fade-in" data-fragment-index="1">Same data</span>
<span class="fragment fade-in" data-fragment-index="2">$+$ same analysis</span>
<span class="fragment fade-in" data-fragment-index="3">$\rightarrow$ Same results</span>

<span class="fragment fade-in" data-fragment-index="4">(from [The Turing Way project](https://the-turing-way.netlify.app/reproducible-research/overview/overview-definitions.html))</span>

Notes:
Reproducibility is when you can take the same data,
run the same analysis on it,
and get the same results out at the end.
This sounds trivial&mdash;if
we can't satisfy this requirement,
are we doing science?
All of science is built on the idea
that we can stand on the shoulders of giants;
if those giants change shape depending on who looks at them,
then we are building on quicksand.

-

## Replicability

New data $+$ same analysis $\rightarrow$ Same results

<br>

## Robustness

Same data $+$ new analysis $\rightarrow$ Same results

Notes:
If we don't have reproducibility,
then these are right out.

-

![Diagram showing four plots with horizontal error bars; the bars from the top plot are projected downward for comparison. The next two agree (and are marked with green check marks) and the last does not agree within errors (marked with a red cross)](./images/reproducibility-within-errors.svg) <!-- .element height="600px" style="margin:100px" --> ![Diagram showing four similar blocks of zeroes and ones. Two are identical to the top one and are marked with a green check mark; one is different by one digit (marked in red) and is marked with a red cross.](./images/bitwise-reproducibility.svg) <!-- .element height="600px" "style="margin:100px" -->

Notes:
There are two main types of reproducibility in this context.
One form is that
you can obtain results that are compatible within errors with the original&mdash;if
your methods don't allow that,
then there is a significant concern over whether you are producing valid science.
The second is that you can obtain every single number identically
down to the last bit,
known as "bitwise reproducibility".
This would be ideal,
there are many cases where it is particularly hard to achieve.

-

## Open Science

The movement to make all research accessible to all levels of society.

![Papers](images/paper.jpg) <!-- .element width="200px" -->&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Experimental Samples](images/test_tube.jpg) <!-- .element width="200px" -->](https://www.publicdomainpictures.net/en/view-image.php?image=302908&picture=filling-up-the-test-tube)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![Code](images/photo_of_code.jpg) <!-- .element width="200px" --> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ![Data](images/photo_of_data.jpg) <!-- .element width="200px" -->

Notes:
In some sense,
this will always be an unachievable ideal to be strived towards.
The more of society we make our data accessible to,
the more overhead costs pile up.
Try making a petabyte of data downloadable to anyone on the internet
without a business model to pay for the bandwidth and long-term fast storage.

-

## [FAIR](https://www.go-fair.org/fair-principles/)

Data and software should be:

- **F**indable
- **A**ccessible
- **I**nteroperable
- **R**eusable

Notes:
Each of these terms has more detailed definitions;
see the [FAIR Principles](https://www.go-fair.org/fair-principles/).

-

## Persistent identifier

- A long-lasting reference to an object.
- Does not change even if the original moves.
- Ideally, resolves in a web browser.

![DOI](./images/doi.svg) <!-- .element class="fragment" -->

Notes:
You're probably familiar with DOIs as journals give them out for articles
(since journals love to reorganise their websites).

---

# Case studies

-

[![Screen shot of the article "the war over supercooled water"](./images/supercooled-water.png) <!-- .element width="1000px" -->](https://physicstoday.scitation.org/do/10.1063/pt.6.1.20180822a/full/)

Notes:
In 2012,
a discrepancy was found between two research groups' results
for computational modelling of part of the phase diagram of water.
It took seven years,
multiple complaints to journals,
and a PhD studentship
to identify that the likely cause was a choice of initialisation function,
because one of the two groups refused to share their code
(i.e. _explain what it was had been done_).
Wouldn't the world be better if the code had been open from the start,
the disagreement resolved over coffee in 2012,
and those energies directed to pushing research forward instead?

-

[![Screen shot of the article "FAQ: Reinhart, Rogoff, and the Excel Error That Changed History"](./images/reinhart-rogoff.png) <!-- .element width="700px" -->](https://www.bloomberg.com/news/articles/2013-04-18/faq-reinhart-rogoff-and-the-excel-error-that-changed-history)

Notes:
In the 2010s,
governments around the world chased a programme of austerity,
justified in part by research indicating that it led to growth.
This could not be reproduced,
as the original analysis,
not shared,
omitted part of the dataset;
when these were included,
the conclusions were no longer supported.
If peer reviewers were able to verify the analysis by reviewing or running the code,
this paper would never have been published.
(Of course,
austerity is ultimately a political and ideological choice,
and it's entirely possible governments would have chosen to do it anyway.)

-

[![Screen shot of the article "Microsoft Excel blamed for gene study errors"](./images/excel-gene.png) <!-- .element width="700px" -->](https://www.bbc.co.uk/news/technology-37176926)

Notes:
Geneticists have been fighting Excel for a long time;
they have now conceded defeat and renamed many genes
to avoid them being confused for dates in English.
(The problem may still remain in other languages,
however!)

-

<!--Process $\rightarrow$ ⬛ $\rightarrow$ 🪄 $\rightarrow$ 💩-->

![Process to black box to magic wand to pile of poo](./images/process-poo.png) <!-- .element width="500px" -->

Notes:
It turns out that when the results are produced magically by a black box,
frequently they may turn out to not be reproducible,
and to be of little value.

-

[![Image of a tweet reading "Another reminder: reviewers and editors need to insist that software be placed in a permanent repository. Not author's web site. Not GitHub.", quoting a second reading "Anyone know where to find the xenograft read detecting software Xenome? Link on the paper is dead."](images/code_archive_tweet.png) <!-- .element:  width="800px" -->](https://twitter.com/michaelhoffman/status/796103749068529667)

Notes:
Author websites can and do go offline when universities reorganise their server setups.
GitHub is a service for development,
and makes no long-term guarantees;
links will break if you change your username.
GitLab almost started purging inactive projects a few years ago;
almost all research outputs will be "inactive" once published!

-

[![Graph showing the importance of research software to researchers](./images/hettrick-importance.png) <!-- .element width="600px" --> &nbsp;&nbsp;&nbsp;&nbsp;![Graph showing the estimated expertise of researchers](./images/hettrick-expertise.png) <!-- .element width="600px" -->](https://slides.com/simonhettrick/software-risks-reproducibility-and-sustainability)

(from [Software Survey 2020, Simon Hettrick](https://slides.com/simonhettrick/software-risks-reproducibility-and-sustainability))

Notes:
Almost all research now relies heavily on software.
A lot fewer researchers feel confident about producing that software.

---

# Modest proposals

-

![Screen shot of arxiv.org](./images/arxiv.png) <!-- .element width="400px" --> ![Screen shot of biorxiv.org](./images/biorxiv.png) <!-- .element width="400px" --> ![Screen shot of medrxiv.org](./images/medrxiv.png) <!-- .element width="400px" -->

Notes:
The increase in the use of preprints goes a long way
to help make narrative outputs more accessible
to those who can't afford to pay journal subscriptions.

-

![Pipline goes paper to reviewer to journal](./images/no-preprint-process.png)

Notes:
Before preprints,
the model was to write a paper,
submit it for peer review,
and then have it appear in a journal.

-

![Pipeline goes paper to both preprint server and reviewer, and from reviewer to both preprint server and journal, and from journal to preprint server](./images/preprint-process.png)

Notes:
Now,
after each of these stages,
a copy can be deposited with a preprint server to be made available openly.
Talk to your librarians about "rights retention" to ensure you're allowed to do this!

-

## Croucher’s law

*“I am an idiot and I will make mistakes”*

&mdash;[Mike Croucher](https://mikecroucher.github.io/MLPM_talk/)

Notes:
Human error is inevitable.
We should plan for it,
rather than hope it doesn't affect us.

-

![Comic exhorting us to "automate ALL the things"](./images/automate.png)

(with apologies to [Hyperbole and a Half](https://hyperboleandahalf.blogspot.com))

Notes:
This doesn't bypass human error,
but does make it more detectable and auditable.
We fix an error once,
then it doesn't happen again
(at least for that workflow).
We miss an error,
someone else can spot later exactly where we went wrong.

-

[![Software Carpentry](./images/swc.svg) <!-- .element width="500px" -->](https://software-carpentry.org) &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [![Data Carpentry](./images/dc.svg) <!-- .element width="300px" -->](https://datacarpentry.org)

Notes:
This requires some programming.
Fortunately,
there are organisations that can help with learning to do so.

-

[![Logo of the Data Stewards Network](./images/data-stewards.svg) <!-- .element width="400px" -->](https://datastewards.net/)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [![Logo of the Society of Research Software Engineering](./images/socrse-knockout.png) <!-- .element width="400px" -->](https://society-rse.org)

Notes:
There is also professionalisation in those who look after data and software,
and train researchers in how to do so.

-

![Papers](./images/paper.jpg) <!-- .element width="100px"  vertical-align="middle" --> ![right arrow](./images/arrow.svg) ![DOI](./images/doi.svg) <!-- .element width="100px"  vertical-align="text-middle" --> 

![Code](./images/photo_of_code.jpg) <!-- .element width="100px"  vertical-align="text-middle" --> <span class="fragment fade-in" data-fragment-index="1"> ![right arrow](./images/arrow.svg) ![DOI](./images/doi.svg) <!-- .element width="100px" vertical-align="text-middle" --></span>

![Data](./images/photo_of_data.jpg) <!-- .element width="100px"  vertical-align="text-middle" --> <span class="fragment fade-in" data-fragment-index="1"> ![right arrow](./images/arrow.svg) ![DOI](./images/doi.svg) <!-- .element width="100px"  vertical-align="text-middle" --></span>

Notes:
Historically,
only narrative outputs (papers) were citable by DOI.
This makes it hard for the importance of data and software to be recognised.
By publishing data and software in places that grant a DOI,
they show up in the same metrics as papers,
so can start to be recognised more.

---

# Technicalities

-

![Image showing serial vs vector computation, `-funsafe-math`, an illustration of a GPU, and the Intel and Arm logos](./images/reproducibility-barriers.svg) <!-- .element width="1200px" -->

Notes:
More things than you would think can stand in the way of bitwise parallelism.
Moving from scalar to vector computation,
such as using the SIMD units on your CPU,
can change the rounding.
This is exacerbated if you enable "unsafe math" optimisations
(not "fun, safe math"!).
Moving to GPU scales this up.
Even switching between different CPU instruction sets can do this.
One example:
in an analysis in Python,
calling one of the Scipy optimisation functions for a specific dataset,
running on Intel the solver converged,
but on Arm it didn't,
leading to a visible
(but compatible within uncertainties)
difference in the final answer.

-

![Diagram of two different software stacks giving different output plots](./images/environment-spec.svg) <!-- .element width="900px" -->

Notes:
Even if you run on the same hardware,
the software stack has a huge impact on your output.
With many libraries,
version differences can give different numerical or visual outputs.
It's generally recommended to define your software environment as data,
such that others can recreate it precisely on their own setup.
Ways of doing this include
environment virtualisation tools like [Conda](https://docs.conda.io/en/latest/),
containerisation tools
like [Docker](https://docker.com)
and [Apptainer](https://apptainer.org),
and functional package managers
like [Nix](https://www.nixos.org)
and [Guix](https://guix.gnu.org).

-

![Diagram of input files leading to a large number of intermediary files, to a larger number of intermediary variables, ultimately to a single plot](./images/workflow-explosion-7.svg) <!-- .element width="1300px" -->

Notes:
Trying to write instructions to carry out each step in a complex analysis
is guaranteed to introduce human error;
remember Croucher's law.
In principle we can encode every step into a single script,
but this can be brittle.
What if we change one data file,
or the format of one plot?
We don't want to have to re-run every step in what could be an expensive analysis.
What if we want to run steps in parallel to make it go faster?
We don't really want to haev to do parallel programming for our analysis.
This is where a "workflow manager" becomes useful.
Rather than having to reimplement every feature from scratch,
we use a set of tools that have already dealt with these problems.
One such tool is [Snakemake](https://snakemake.github.io);
[a guide on doing this in a lattice context is available](https://edbennett.github.io/snakemake-novice-lattice)
but there are others that have similar functionality.

-

[![Screen shot of zenodo.org](./images/zenodo.png) <!-- .element width="1000px" -->](https://zenodo.org)

Notes:
Once your workflow and data can reproduce your findings,
you still need to publish it somewhere so others can verify and cite it.
One example of a suitable venue to publish data and software,
that provides a DOI,
and makes a commitment to long-term availability of the published work,
is Zenodo,
run by CERN.

---

## Conclusions

- If your results aren't reproducible,<br>
  are you doing science?
  
- If your workflows aren't automated,<br>
  human error is present in your results
  
- If your data and workflows aren't public,<br>
  can reviewers and readers trust them?

-

## Further reading

- [Lattice Virtual Academy lectures<br>on reproducibility and open science](https://sites.google.com/view/lattice-virtual-academy/topics/open-science)
- [The TELOS Collaboration Approach<br>to Reproducibility and Open Science](https://arxiv.org/abs/2504.01876)
- [The Turing Way](https://the-turing-way.netlify.app/reproducible-research/)
