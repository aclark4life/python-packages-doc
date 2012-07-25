
Frequently Asked Questions
==========================

If your quesiton is not answered here, please `open a ticket`_.

Q: How does pythonpackages.com differ from the Python Package Index (PyPI)?
---------------------------------------------------------------------------

**A:** pythonpackages.com is not a package index, i.e. we do not host any files for download. We consume their (PyPI) API to display useful information about packages, as well as provide additional services to Python programmers to help package and release their software.

Q: How does pythonpackages.com differ from Bitbucket, GitHub, etc?
------------------------------------------------------------------

**A:** pythonpackages.com is not a software repository. We consume their (GitHub) API to provide services to Python programmers to help package and release their software.

.. _`open a ticket`: http://bitbucket.org/pythonpackages/pythonpackages.com/issues/new

Q: How do you make money?
-------------------------
**A:** Developers are encouraged to use the free plan which includes a single "package slot" to evaluate the service. If the service provides significant value, they are encouraged to purchase a paid plan which includes some number of paid slots, depending on the plan. Additionally, paid plans allow access to some number of GitHub organization repositories, depending on the plan.

Q: Is pythonpackages.com open source?
-------------------------------------

**A:** The web application that powers pythonpackages.com is not open source, however it uses open source software where and when applicable, and permissible by license, in order to facilitate its operation. Furthermore, pythonpackages.com has a large committment to the open source software community in general, and strives to contribute as much as possible. All of pythonpackages.com's open source offerings are made available here: https://github.com/pythonpackages.

Q: What does pythonpackages.com do for me that I can't do myself?
-----------------------------------------------------------------

**A:** In order to publish software Python developers are required to know a tremendous amount of information about the available packaging framework(s) e.g. distutils, setuptools, distribute, etc. Many Python programmers simply do not know or care to know about Python packaging. pythonpackages.com provides services to help decrease the amount of knowledge necessary to publish Python software. Additionally, pythonpackages.com enables so-called "cloud releases" in which publishing can be done entirely "in the cloud" i.e. without requiring a local development environment. One popular scenario::

    Developer "Mary" is the author of "Mary's Awesome App". Mary develops her application on GitHub, where she can easily collaborate with other like-minded developers.

    One day Mary is on vacation, but still checking her email on her iPhone, when she receives a "Pull request" from "Josh" who is another open source developer on GitHub. Josh has informed Mary of a critical bug fix he made to her software. Further, he indicates that the tests have passed on Travis CI and the request is ready to be merged and released.

    Mary is naturally skeptical at first. The "old" Mary would never have considered performing a release without testing on her laptop! However, since her code has 100% test coverage, and Josh is a reliable community member, and she can ensure that the tests have passed she happily agrees to perform a release. Using the mobile-friendly UI on her iPhone, Mary presses the "Tag and release" button on pythonpackages.com to publish a new release of Mary's Awesome App from GitHub to the Python Package Index. Mary goes back to her vacation. Josh goes back to fixing bugs. And users of Mary's Awesome App are delighted about the new release.
