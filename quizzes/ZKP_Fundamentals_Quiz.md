# ZKP Fundamentals Quiz

1. Which of the following problems of blockchain can be solved with zero-knowledge proofs?
    
    Note: There might be multiple correct options
    
    A) Privacy
    
    B) Scalability
    
    C) Decentralisation
    
    D) All of the above
    
    Answer: A, B
    
    Zero-knowledge proofs provide privacy because the inputs for computation can be kept private and also provide scalability as the verifier need not do the complete computation again to verify that the computation was done correctly.
    
2. Which of these is NOT a required property of zero-knowledge proof protocol?
    
    A) Completeness
    
    B) Soundness
    
    C) Zero-Knowledge
    
    D) Non-Interactivity
    
    Answer: D
    
    Zero-knowledge protocols can be non-interactive or interactive.
    
3. Soundness is a property that states, that if a proof is valid it must be accepted by the verifier.
    
    A) True
    
    B) False
    
    Answer: False
    
4. What is the main difference between an interactive and non-interactive zero-knowledge proof?

    A) Interactive proofs require communication between the prover and verifier, while non-interactive proofs do not

    B) Interactive proofs are more secure than non-interactive proofs

    C) Interactive proofs are more efficient than non-interactive proofs

    D) None of the above
    
    
    Answer: A
    

5. Which of the following is **generated** in the setup phase of zk-SNARKs?
    
    A) Proving Key
    
    B) Verification Key
    
    C) A secret value (lambda)
    
    D) None of the above
    
    Answer: A, B
    
6. What is the correct order of steps for a zkSNARK protocol?
    
    a. Generate Proof

    b. Verify the Proof

    c. Generate the Program/Constraints
    
    d. Generate Keys
    
    A) c, d, a, b
    
    B) d, c, b, a
    
    C) d, c, a, b
    
    D) c, d, b, a
    
    Answer: A)
    
7. What is the term for the secret information that the prover knows in a zero-knowledge proof?
    
    A) Witness

    B) Statement

    C) Commitment

    D) Challenge

    Answer: A)

8. Proofs generated using zkSNARK are immune to quantum computing threats.
    
    A) True
    
    B) False
    
    Answer: B)
    
    STARK proofs are quantum proof because they use hashes, however SNARK proofs are not quantum secure.