-----------


# Your turn now!

<img src="https://media.giphy.com/media/13GIgrGdslD9oQ/giphy.gif" width=50%/>

  - [1) The Simulator starts today!](#1-the-simulator-starts-today)
  - [2) DevOps Principles](#2-devops-principles)
  - [3) Introduce a DB abstraction layer in your _ITU-MiniTwit_](#3-introduce-a-db-abstraction-layer-in-your-itu-minitwit)
  - [4) Make your configuration management scripts idempotent](#4-make-your-configuration-management-scripts-idempotent)
  - [5) Software Maintenance](#5-software-maintenance)


## 1) The Simulator starts today!

We will start the simulator **today** in the exercise session (in between 15:00 and 16:00).

In case you have not done so yet, send a pull request to `repositories.py` in our central repository: https://github.com/itu-devops/MSc_lecture_notes/blob/master/repositories.py!

Add two URLs:

  * One to your running applications (edit `"http://<minitwit_application_url>"`)
  * Another one to the simulator API endpoint (edit `"http://<sim_api_url>"`)


## 2) DevOps Principles

Consider how much you as a group adhere to the "*Three Ways*" characterizing DevOps (from _"The DevOps Handbook"_):

  * Flow
  * Feedback
  * Continual Learning and Experimentation

Map what you are doing with regards to each principle.
In case you realize you are not doing something for a principle change the way you are working as a group accordingly.


## 3) Introduce a DB abstraction layer in your _ITU-MiniTwit_.

Introduce a DB abstraction layer so that you do not directly communicate with the DB anymore.
That is, you should not have any SQL queries in your application anymore after this refactoring.
Instead, introduce for example an Object-relational mapping (ORM) framework to your application so that you decouple it from the actual DBMS.


## 4) Make your configuration management scripts idempotent

Make sure that all configuration management code is idempotent, i.e., it can be run repeatedly without undesired side-effects leaving your systems in undesired states.

Optionally, if you consider that configuration management tools like Ansible, Chef, Puppet, etc. are more suitable than plain shell scripts, migrate your configuration management code to one of these.
In the following, you find a list of potential alternative configuration management tools:

  * [Ansible](https://docs.ansible.com/projects/ansible/latest)
  * [Chef](https://docs.chef.io/)
  * [Puppet](https://www.puppet.com/docs/index.html)
  * [Salt](https://docs.saltproject.io/en/latest/contents.html)
  * [PyInfra](https://docs.pyinfra.com/en/3.x/)
  * [Pulumi](https://www.pulumi.com/docs/)



## 5) Software Maintenance

### a) Fix issues as they occur

From now on we are in software maintenance. That is, fix issues of your version of _ITU-MiniTwit_ as soon as possible. Likely, after the simulator is started you will experience some issues in your systems. Just fix them as soon as you realize them.

For example, you will be able to see status and potential errors as the simulator 'sees' them [here](http://138.68.85.121/status.html).

Continue to release (now likely automatically) whenever new features and bug-fixes are ready (least once per week).

### b) Add missing features

Likely, your implementations are not complete yet.
They lack some features that were present in the version that you took over, or you have some features that you would like to add.

Add missing features continuously from now on and during the following weeks.