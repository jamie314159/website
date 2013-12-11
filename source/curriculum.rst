Curriculum
==========

The curriculum will be constantly evolving as we develop this course. The
first unit will be an overview of what students will need to know in order to
understand the deeper technical concepts which will be covered later.

Here's what we're hoping to mentor and teach students about:

#. Linux Basics
#. Basic System Administration
#. Basic FOSS Development Methodologies
#. Base infrastructure services for any organization (DNS, Email, etc)
#. Building a mock infrastructure for a mock company from top to bottom

.. note:: Note that the curriculum past week 4 is currently under development. Lesson
    titles are included to provide an overview of what we'll cover, but specific
    content is likely to get moved around between lessons depending on what we
    learn about the pace of the class during the first few weeks.

    Slide content will be linked here as soon as it's drafted, but only finalized
    1-2 weeks before the lessons when it's presented.

:doc:`Lesson 1: The Very Basics <01_the_very_basics>`
-----------------------------------------------------

Shell, virtualbox+vagrant, IRC.

- 6pm 11/7/2013, KEC1007. 34 people attended.
- `Video <http://youtu.be/UiiPiIoTxnw>`_

:doc:`Lesson 2: Single System Fundamentals <02_single_system_fundamentals>`
---------------------------------------------------------------------------

Users, Groups, and package management

- 6pm 11/14/2013, KEC1001. 27 people showed up.
- `Video <http://youtu.be/0mWSep_qmJM>`_

:doc:`Lesson 3: Files <03_editors_git>`
---------------------------------

Version control & text editors (Vim)

- `Part 1, text editors video <https://www.youtube.com/watch?v=4ce3P_mvOvA>`_ 
- `Part 2, version control video <https://www.youtube.com/watch?v=vBeAP7i_mPg>`_

Lesson 4: Scripting & Troubleshooting
-------------------------------------

.. note:: week 1, 1/9/2014

- slides: :doc:`troubleshooting`

- log files
- git bisect, git log, git blame
- scientific method (small changes)

Lesson 5: Services and deploying a web app
------------------------------------------

.. note:: pwnguin pulls talk from harvard extension web dev class (please
          link)
    1/16/2014

- services, init scripts
- we'll provide a simple web app (hello world selector)
- ops: more about HTTP?
- languages
    - hello world
    - "single-serving" web sites

Lesson 6: Boot and the filesystem hierarchy, and more app dev
-------------------------------------------------------------

.. note:: more ops-focused
    1/30/2014

- grub, filesystem stuff based roughly on Frostsnow's talk
- basics of kernel and differences between virtualization/physical
  (the picture that kevin draws)
- CS311 in a very small nutshell

- build a piece of web app to perform systems monitoring based on ^^

Lesson 7: integration: connecting app to DB
-------------------------------------------

.. note:: more dev-focused
    2/6/2014

- explain what DBs are and why we need them (transactions, relations, indices,
  performance)
- set up DB instance
- connect app to DB
- show manual queries for doing things
- show what happens when app does things
- teach mysql & postgres like vim & emacs (only install _____ right now)

Lesson 8: Security & Authentication
-----------------------------------

.. note:: 2/13/2014

- key pairs
- ssh keys (passphrase vs none; automation; authorized_keys)
- GPG keys, signing stuff, publishing to keyservers
- certificates (SSL/TLS)

- web app security
    - parameterize or sanitize inputs
    - SQL injection
    - XSS, csrf tokens
    - https://www.owasp.org/index.php/Top_10_2013-Top_10
    - filesystem & user permissions (remember lesson 2?)

- mention social engineering type attacks

:doc:`security_auth`

Lesson 9: Networking overview
-----------------------------

:doc:`networking_overview`

Lesson 10: Services
-------------------

Note: This will take several weeks, probably one week per service that we'll
study



Lesson 11: Configuration Management & Cron
------------------------------------------

.. note:: 3/6/2014

:doc:`config_mgmt_cron`

Lesson 12: Infrastructure Design
--------------------------------

:doc:`infra_design`
