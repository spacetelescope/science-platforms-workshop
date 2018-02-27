CafeCon, Mon, Feb 26, 2-3pm
---------------------------

Initial questions
-----------------

How do we manage users?

How do we prevent/detect bad actions?

*   Intentional and unintentional

How do we communicate with users about noncompliance?

With code to data:

*   What code?  From whom?

Levels of concern
-----------------

*   Integrity of archive data
*   Privacy between/among users
    *   Proprietary data for users or groups
    *   General user privacy

*   Overuse of resources
*    Misuse (deliberate) of resources

Specific concerns
-----------------

*   Is there a way to prevent user access to root in Docker containers?  Background:  Some HPC providers don't provide Docker containers.  Singularity instead which runs everything as the user, nothing as "root", so less exposure.
*   Re preserving containers over time:  How do we deal with old containers that have known vulnerabilities?
*   How to detect undesired actions?
    *   How much use is overuse?
    *   During overuse, what do we do?
*   AuthN
*   AuthZ
*   Protecting users credentials, esp. when they delegate authority to us to access another service

Mitigations
-----------

*   Follow general security best practices
    *   Safe coding
    *   Code reviews
*   Keep up to date with container security reports and patches.
*   Run tools to look for vulnerabilities (e.g., look for SQL injection)
    *   Generic tools may not cover Jupyter notebooks well, esp. in our astro use cases.
*   Require account
    *   If ID of human is known, this is more effective, but it still helps either way.
*   Logging can help
    *   Look for bad patterns, e.g., lots of compute with no local data acess
*   VO is looking at standardizing group management, which can span multiple AuthN techniques.  (Associating multiple accounts still necessary.  Up to host as to who/what IDs they trust.)
*   Limit parallel jobs.  
      
    

Overall suggestions
-------------------

*   Prioritize mitigations based on consequences and likelihood.

  
