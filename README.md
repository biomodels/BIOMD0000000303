# BIOMD0000000303: Complement_System

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000303.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000303.git@20140916`

## Usage

Importing the model package.

`import BIOMD0000000303 as model`

Get the SBML string from the model

`print model.sbmlString`

If [python-libsbml](https://pypi.python.org/pypi/python-libsbml) bindings are
installed, the libsbml.SBMLDocument object is also accessible

`model.sbml`


# Model Notes


This is the continuous deterministic (ODE) model of the complement system
described in the article:  
**Computational and Experimental Study of the Regulatory Mechanisms of the Complement System.**   
Liu B, Zhang J, Tan PY, Hsu D, Blom AM, Leong B, Sethi S, Ho B, Ding JL and
Thiagarajan PS. PLoS Comp. Bio. 2011 Jan. 7:1; doi:[10.1371/journal.pcbi.10010
59](http://dx.doi.org/10.1371/journal.pcbi.1001059)

Abstract:  
The complement system is key to innate immunity and its activation is
necessary for the clearance of bacteria and apoptotic cells. However,
insufficient or excessive complement activation will lead to immune-related
diseases. It is so far unknown how the complement activity is up- or down-
regulated and what the associated pathophysiological mechanisms are. To
quantitatively understand the modulatory mechanisms of the complement system,
we built a computational model involving the enhancement and suppression
mechanisms that regulate complement activity. Our model consists of a large
system of Ordinary Differential Equations (ODEs) accompanied by a dynamic
Bayesian network as a probabilistic approximation of the ODE dynamics.
Applying Bayesian inference techniques, this approximation was used to perform
parameter estimation and sensitivity analysis. Our combined computational and
experimental study showed that the antimicrobial response is sensitive to
changes in pH and calcium levels, which determines the strength of the
crosstalk between CRP and L-ficolin. Our study also revealed differential
regulatory effects of C4BP. While C4BP delays but does not decrease the
classical complement activation, it attenuates but does not significantly
delay the lectin pathway activation. We also found that the major inhibitory
role of C4BP is to facilitate the decay of C3 convertase. In summary, the
present work elucidates the regulatory mechanisms of the complement system and
demonstrates how the bio-pathway machinery maintains the balance between
activation and inhibition. The insights we have gained could contribute to the
development of therapies targeting the complement system.

Comment:  
Reproduction of figures in the article:  
Figure 5: the effects of C4BP  
Fig 5A: set initial concentrations PC=0.0327796, GlcNac=0, vary the initial
concentration of C4BP from 2.6 to 2600 using parameter scan  
Fig 5B: set initial concentrations PC=0, GlcNac=0.0327796, vary the initial
concentration of C4BP from 2.6 to 2600 using parameter scan  
Figure 6: knockout simulations  
Set PC=0.0327796, GlcNac=0  
Fig 6A: kf01=0, kf02=0  
Fig 6B: kf04=0, kf06=0, kf07=0  
Fig 6C: kf05=0  
Fig 6D: kf03=0

This model originates from BioModels Database: A Database of Annotated
Published Models (http://www.ebi.ac.uk/biomodels/). It is copyright (c)
2005-2011 The BioModels.net Team.  
For more information see the [terms of
use](http://www.ebi.ac.uk/biomodels/legal.html).  
To cite BioModels Database, please use: [Li C, Donizelli M, Rodriguez N,
Dharuri H, Endler L, Chelliah V, Li L, He E, Henry A, Stefan MI, Snoep JL,
Hucka M, Le Novère N, Laibe C (2010) BioModels Database: An enhanced, curated
and annotated resource for published quantitative kinetic models. BMC Syst
Biol., 4:92.](http://www.ncbi.nlm.nih.gov/pubmed/20587024)


