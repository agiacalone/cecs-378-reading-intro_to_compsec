# CECS 378 Reading Assignment: Introduction to Computer Security
## 20 points

### Assignment Description
Answer the following questions from the Chapter 1 reading from your textbook. You may work on these questions with one or two other partners, but *all* students must submit the document individually in their own repositories along with each student's name documented with the submission.


1. Define the term *computer security*.

2. What is the difference between passive and active security threats?

3. Explain the difference between an attack surface and an attack tree.

4. Consider an automated teller machine (ATM) in which users provide a personal identification number (PIN) and a card for account access. Give examples of confidentiality, integrity, and availability requirements associated with the system and, in each case, indicate the degree of importance of the requirement.

5. Repeat question #4 for a telephone switching system that routes calls through a switching network based on the telephone number requested by the caller.

6. List and briefly define the fundamental security design principles.

7. Consider a desktop publishing system used to produce documents for various organizations.
    1. Give an example of a type of publication for which confidentiality of the stored data is the most important requirement.
    2. Give an example of a type of publication in which data integrity is the most important requirement.
    3. Give an example in which system availability is the most important requirement.

8. For each of the following assets, assign a low, moderate, or high impact level for the loss of confidentiality, availability, and integrity, respectively. Justify your answers.
    1. An organization managing public information on its Web server.
    2. A law enforcement organization managing extremely sensitive investigative information.
    3. A financial organization managing routine administrative information (not privacy-related information).
    4. An information system used for large acquisitions in a contracting organization contains both sensitive, pre-solicitation phase contract information and routine administrative information. Assess the impact for the two data sets separately and the information system as a whole.
    5. A power plant contains a SCADA (supervisory control and data acquisition) system con- trolling the distribution of electric power for a large military installation. The SCADA system contains both real-time sensor data and routine administrative information. As- sess the impact for the two data sets separately and the information system as a whole.

9. Develop an attack tree for gaining access to the contents of a physical safe.

10. Consider the following general code for allowing access to a resource:
    ```
    DWORD dwRet = IsAccessAllowed(...);
    if (dwRet == ERROR_ACCESS_DENIED) { // Security check failed.
    // Inform user that access is denied. } else {
    // Security check OK.
    }
    ```
    1. Explain the security flaw in this program.
    2. Rewrite the code to avoid the flaw
    (Hint: Consider the design principle of fail-safe defaults).

### Deliverables
Commit the answers to the questions in a readable file to your git repository by the due date and time indicated with your repository. Approved file submission formats are: .txt, .md, .pdf. .html (renderable) or anything that is web-readable on Github. Other formats will only be accepted with explicit approval.
