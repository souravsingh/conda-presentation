#### Conda Forge- Community driven packaging for Anaconda.
[@MrSouravSingh](https://twitter.com/MrSouravSingh)

---

#### Inspiration Behind Conda.

- Cross-platform support
- Language agnosticism
- Does not require admin rights
- Easy to use.

---

#### What is Conda?

Open-source packaging system developed by Continuum Analytics.

---

#### Why use conda?

- Easy to create virtual environments which can be reproducible.
- Easy installation of packages.
- Supports packages from multiple languages like Python, R, Fortran, C, C++ and so on.

---

#### Problems with existing conda build structure.

- Getting latest tools not packaged by Continuum.
- Hosting packages.
- Building the recipes so that they are compatible with other systems and with packages available in Anaconda.  
---

#### The Solution

Conda-forge organization was created with to be a transparent, open community led organization, to build conda packages and, 
hopefully, provide a stable source for packages while reducing the effort duplication and recipe fragmentation.

---
#### What do we mean by it?

Have a community driven ""channel" for conda and a community process for submission, verification and building of the packages.

[https://conda-forge.github.io](https://conda-forge.github.io)

---
### Payoff Matrix

![IMAGE](assets/payoff_matrix.png)

---
#### More on Prisoner's Dilemma
<img src="assets/valentine_dilemma.png" height="450"/>

Taken from [https://xkcd.com/1016/](https://xkcd.com/1016/)
---
#### Iterated Prisoner's Dilemma

1. Started out by Robert Axelrod as a student in 1962.
2. [Axelrod1980](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.665.7955&rep=rep1&type=pdf): 15 strategies
3. [Axelrod1980b](http://journals.sagepub.com/doi/abs/10.1177/002200278002400301): 65 strategies

---

### IPD in Python
<img src="http://vknight.org/Talks/2017-02-13-The-Axelrod-library/static/axelrod-tweet.png" alt="Drawing" style="height: 480px;"/>
---

### Basic Strategy for IPD

```python
class TitForTat(Player):
    """A player starts by cooperating and then mimics previous move by opponent."""

    name = 'Tit For Tat'
    classifier = {
        'memory_depth': 1,  # Four-Vector = (1.,0.,1.,0.)
        'stochastic': False,
        'inspects_source': False,
        'manipulates_source': False,
        'manipulates_state': False
    }

    @staticmethod
    def strategy(opponent):
        return 'D' if opponent.history[-1:] == ['D'] else 'C'
```
---

#### Demo time!

---
<img src="http://axelrod-tournament.readthedocs.io/en/latest/_images/strategies_std_reproduce.svg" width=800>
---

The Axelrod library

Greet us at [Gitter!!](https://gitter.im/Axelrod-Python/Axelrod)

Docs- [axelrod.readthedocs.io](axelrod.readthedocs.io)

---

Thanks to Axelrod-Python community, especially to Dr. Vincent Knight for the help!!

---

Thank you!

---
