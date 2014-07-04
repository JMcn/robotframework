Introduction
------------

Robot Framework is a Python-based, extensible keyword-driven test
automation framework for end-to-end acceptance testing and
acceptance-test-driven development (ATDD). It can be used for testing
distributed, heterogeneous applications, where verification requires
touching several technologies and interfaces.

.. contents::
   :depth: 2 
   :local: 

Why Robot Framework?
~~~~~~~~~~~~~~~~~~~~

- Enables easy-to-use tabular syntax for `creating test cases`_ in a uniform
  way.

- Provides ability to create reusable `higher-level keywords`_ from the
  existing keywords.

- Provides easy-to-read result reports_ and logs_ in HTML format.

- Is platform and application independent.

- Provides a simple `library API`_ for creating customized test libraries
  which can be implemented natively with either Python or Java.

- Provides a `command line interface`__ and XML based `output files`_  for 
  integration into existing build infrastructure (continuous integration 
  systems).

- Provides support for Selenium for web testing, Java GUI testing, running 
  processes, Telnet, SSH, and so on.

- Supports creating `data-driven test cases`__.

- Has built-in support for variables_, practical particularly for testing in
  different environments. 

- Provides tagging__ to categorize and `select test cases`__ to be executed. 

- Enables easy integration with source control: `test suites`_ are just files
  and directories that can be versioned with the production code.

- Provides `test-case`__ and `test-suite`__ -level setup and teardown.

- The modular architecture supports creating tests even for applications with
  several diverse interfaces.

__ `Executing test cases`_
__ `Data-driven style`_
__ `Tagging test cases`_
__ `Selecting test cases`_
__ `Test setup and teardown`_
__ `Suite setup and teardown`_


High-level architecture
~~~~~~~~~~~~~~~~~~~~~~~

Robot Framework is a generic, application and technology independent
framework. It has a highly modular architecture illustrated in the
diagram below.

.. figure:: src/GettingStarted/architecture.png

   Robot Framework architecture

The `test data`_ is in simple, easy-to-edit tabular format. When
Robot Framework is started, it processes the test data, `executes test
cases`__ and generates logs and reports. The core framework does not
know anything about the target under test, and the interaction with it
is handled by `test libraries`__. Libraries can either use application
interfaces directly or use lower level test tools as drivers.

__ `Executing test cases`_
__ `Creating test libraries`_


Screenshots
~~~~~~~~~~~

Following screenshots show examples of the `test data`_ and created
reports_ and logs_.

.. figure:: src/GettingStarted/testdata_screenshots.png

   Test case files

.. figure:: src/GettingStarted/screenshots.png

   Reports and logs


Getting more information
~~~~~~~~~~~~~~~~~~~~~~~~

Project pages
'''''''''''''

The number one place to find more information about Robot Framework
is the project web site at http://robotframework.org. This User Guide is
naturally available there but you can also find more documentation__,
an `issue tracker`__, downloads__, `source code`__ and links to other
related projects. Robot Framework is hosted on `Google Code`__ which
provides excellent free services for open source projects.

__ http://code.google.com/p/robotframework/wiki/DocumentationIndex
__ http://code.google.com/p/robotframework/issues
__ http://code.google.com/p/robotframework/downloads
__ http://code.google.com/p/robotframework/source
__ http://code.google.com

Mailing lists
'''''''''''''

There are several Robot Framework mailing lists where to ask and
search for more information. The mailing list archives are open for
everyone (including the search engines) and everyone can also join
these lists freely. Only list members can send mails, though, and to
prevent spam new users are moderated which means that it might take a
little time before your first message goes through.  Do not be afraid
to send question to mailing lists but remember `How To Ask Questions
The Smart Way`__.

robotframework-users__
   General discussion about all Robot Framework related
   issues. Questions and problems can be sent to this list. Used also
   for information sharing for all users.

robotframework-announce__
    An announcements-only mailing list where only moderators can send
    messages. All announcements are sent also to the
    robotframework-users mailing list so there is no need to join both
    lists.

robotframework-devel__
   Discussion about Robot Framework development. 

robotframework-commit__
   Automatically generated mails about commits to the version control
   system, build results, new and edited issues, and so on. Can be used to
   follow Robot Framework development.

__ http://www.catb.org/~esr/faqs/smart-questions.html
__ http://groups.google.com/group/robotframework-users 
__ http://groups.google.com/group/robotframework-announce
__ http://groups.google.com/group/robotframework-devel 
__ http://groups.google.com/group/robotframework-commit