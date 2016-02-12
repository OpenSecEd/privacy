Module: Privacy (privacy)
===============================================================================

This is a learning module focusing on Privacy.  It's aim is to cover Privacy 
Enhancing Technologies (PETs) and techniques for privacy-preserving 
design.

The module is part of the [Open Security Education][OpenSecEd] project and the 
maintainer is [Daniel Bosk][Maintainer].  The latest release can be found under 
[releases][Releases].  You can safely link directly to the PDFs found there.

[OpenSecEd]: https://github.com/OpenSecEd
[Maintainer]: https://github.com/dbosk
[Releases]: https://github.com/OpenSecEd/privacy/releases


File Structure and Building
-------------------------------------------------------------------------------

*To build* the PDFs, after cloning the repository you must clone its required 
submodules:
```shell
$ git submodule update --recursive --init
```
Then you can go into the directory of the desired document and run `make`.
The source files are structured as follows:

- `diffpriv` contains a learning session for differential privacy.  It's based 
  on a few papers illustrating a variety of uses.

In each directory the files are structured as follows:

- `<name>-content.tex` contains the main content, this is made to be included 
  into an llncs-style proceedings document.
- `<name>-notes.tex` is the main code for compiling the notes.
- `<name>-slides.tex` is the main code for compiling the slides.
- `aims.tex` is an itemized list of the intended learning outcomes, as such it 
  can be included in another document summarizing the list of intended learning 
  outcomes.
- `abstract.tex` is an abstract of the lecture, assignment, or similar, and 
  covers the required reading instructions, thus you can include these in 
  a study guide containing all reading instructions for the course.
- `<name>.bib` contains the bibliography entries, thus this file can be 
  included along with the reading instructions.


*To contribute*, please [fork the repository][ForkARepo], make your changes, 
commit them and then create a [pull request][PullRequest] in the original 
repository.

[ForkARepo]: https://help.github.com/articles/fork-a-repo/
[PullRequest]: https://help.github.com/articles/using-pull-requests/
