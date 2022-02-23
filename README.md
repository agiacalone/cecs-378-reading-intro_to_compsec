# CECS 378 Reading Assignment: Cryptograpgy
## 20 points

### Assignment Description
Answer the following questions from the Chapter 2, 20, and 21 reading from your textbook. You may work on these questions with one or two other partners, but *all* students must submit the document individually in their own repositories along with each student's name documented with the submission.

1. How many keys are required for two people to communicate via a symmetric cipher?

2. What is a message authentication code?

3. What are the principal ingredients of a public-key cryptosystem?

4. With the ECB mode, if there is an error in a block of the transmitted ciphertext, only the corresponding plaintext block is affected. However, in the CBC mode, this error propagates. For example, an error in the transmitted C1 (Figure 20.6, pg. 622 in CSPaP) obviously corrupts P1 and P2.
   1. Are any blocks beyond P2 affected?
   2. Suppose that there is a bit error in the source version of P1. Through how many cipher-text blocks is this error propagated? What is the effect at the receiver?

5. You want to build a hardware device to do block encryption in the cipher block chaining (CBC) mode using an algorithm stronger than DES. 3DES is a good candidate. Figure 20.11 on pg. 632 in CSPaP shows two possibilities, both of which follow from the definition of CBC. Which of the two would you choose:
   1. For security?
   2. For performance?
   3. And answer why for each.
      
6. Padding may not always be appropriate. For example, one might wish to store the encrypted data in the same memory buffer that originally contained the plaintext. In that case, the ciphertext must be the same length as the original plaintext. A mode for that purpose is the ciphertext stealing (CTS) mode. Figure 20.12a on pg. 633 in CSPaP shows an implementation of this mode.
   1. Explain how it works.
   2. Describe how to decrypt `Cn−1` and `Cn`.

7. It is possible to use a hash function to construct a block cipher with a structure similar to DES. Because a hash function is one way and a block cipher must be reversible (to decrypt), how is it possible?

8.  Perform encryption and decryption using the RSA algorithm for the following:
    1.  `p=3`; `q=11`, `e=7`, `M=5`
    2.  `p=5`; `q=11`, `e=3`, `M=9`
    3.  `p=7`; `q=11`, `e=17`, `M=8`
    4.  `p=11`; `q=13`, `e=11`, `M=7`
    5.  `p=17`; `q=31`, `e=7`, `M=2`

<<<<<<< HEAD
9.  Suppose we have a set of blocks encoded with the RSA algorithm and we do not have the private key. Assume `n=pq`, `e` is the public key. Suppose also someone tells us they know one of the plaintext blocks has a common factor with `n`. Does this help us in any way?
=======
7. Consider a desktop publishing system used to produce documents for various organizations.
    a. Give an example of a type of publication for which confidentiality of the stored data is the most important requirement.
    b. Give an example of a type of publication in which data integrity is the most important requirement.
    c. Give an example in which system availability is the most important requirement.

8. For each of the following assets, assign a low, moderate, or high impact level for the loss of confidentiality, availability, and integrity, respectively. Justify your answers.
    1. An organization managing public information on its Web server.
    2. A law enforcement organization managing extremely sensitive investigative information.
    3. A financial organization managing routine administrative information (not privacy-related information).
    4. An information system used for large acquisitions in a contracting organization contains both sensitive, pre-solicitation phase contract information and routine administrative information. Assess the impact for the two data sets separately and the information system as a whole.
    5. A power plant contains a SCADA (supervisory control and data acquisition) system con- trolling the distribution of electric power for a large military installation. The SCADA system contains both real-time sensor data and routine administrative information. Assess the impact for the two data sets separately and the information system as a whole.

9. Develop an attack tree for gaining access to the contents of a physical safe.

10. Consider the following general code for allowing access to a resource:
    ```
    DWORD dwRet = IsAccessAllowed(...);
    if (dwRet == ERROR_ACCESS_DENIED) { // Security check failed.
    // Inform user that access is denied. } else {
    // Security check OK.
    }
    ```
    a. Explain the security flaw in this program.
    b. Rewrite the code to avoid the flaw
    (Hint: Consider the design principle of fail-safe defaults).
>>>>>>> parent of 0801144 (fixed number formating)

### Deliverables
Commit the answers to the questions in a readable file to your git repository by the due date and time indicated with your repository. Approved file submission formats are: .txt, .md, .pdf. .html (renderable) or anything that is web-readable on Github. Other formats will only be accepted with explicit approval.
