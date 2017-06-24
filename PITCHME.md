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
### conda-forge channel

- More than 60 contributors.
- More than 400 packages.
- Available for: Linux-64, Windows-32/64, and OS X
- Install using: ``conda install -c conda-forge package_name``

---
#### How to contribute?

- Make PR for adding new packages.
- Report problems with existing packages.
- Request for packages.

---
#### Submit recipe to conda-forge

- Fork [https://github.com/conda-forge/staged-recipes](https://github.com/conda-forge/staged-recipes)
- Edit the example YAML recipe and create PR.
- Recipe will be built on multiple CI services and once merged, trigger creation of feedstock repository on Github.
- At the feedstock repository, recipe is re-built and uploaded to the conda-forge channel.

---
Where to find us?

[Github](https://github.com/conda-forge)

[Gitter](https://gitter.im/conda-forge/conda-forge.github.io)

[Mailing List](https://groups.google.com/forum/#!forum/conda-forge)
---
