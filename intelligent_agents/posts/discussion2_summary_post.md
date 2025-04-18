## Collaborative Discussion 2: Agent Communication Languages (Summary Post)  


This discussion explored the advantages and limitations of Agent Communication Languages (ACLs), with a focus on KQML, and how they compare to traditional method invocation approaches in programming languages like Python and Java. In my initial post, I highlighted KQML’s strengths in supporting asynchronous, decoupled communication through structured performatives, making it suitable for distributed and autonomous multi-agent systems (Mayfield et al. 1996; Labrou et al, 1999). I also noted practical challenges such as inconsistent semantic interpretation and limited standardisation, which affect interoperability across diverse agent implementations (Singh, 1998).

Peer contributions added other dimensions. Rodrigo outlined the historical tension between ACLs and traditional programming languages, noting that modern frameworks like JADE and PADE, built on Java and Python, have addressed many practical limitations of ACLs by offering better integration, tooling, and standardised communication protocols. Abdulhakim’s post further stressed the significance of loose coupling in agent systems. It argued that while method invocation is suitable for tightly coupled components, it limits flexibility and adaptability at scale (Mämmelä et al., 2023).

While ACLs like KQML have lost prominence in some domains, they remain relevant in scenarios where semantic-level communication is required, such as negotiation, coordination, or belief sharing in BDI agents (Wooldridge, 2009). Agent-based design is increasingly being used alongside modern programming tools, combining agent principles with the practical features of common programming languages.

In conclusion, this discussion reinforced the importance of choosing communication approaches based on system context. ACLs offer expressiveness and autonomy in distributed environments, while method invocation remains efficient for simpler, tightly bound systems. Future agent design will likely continue to blend both approaches for scalability, maintainability, and clarity.


**References**

Labrou, Y., Finin, T. & Peng, Y., 1999. Agent communication languages: the current landscape. IEEE Intelligent Systems and their Applications, 14(2), pp.45–52. Available at: http://dx.doi.org/10.1109/5254.757631.

Mämmelä, A., Riekki, J., and Kiviranta, M. (2023). Loose Coupling: An Invisible Thread in the History of Technology. IEEE Access, 11, 59456–59482. https://doi.org/10.1109/ACCESS.2023.3284685

Mayfield, J., Labrou, Y. & Finin, T., 1996. Evaluation of KQML as an agent communication language. In Intelligent Agents II Agent Theories, Architectures, and Languages. Lecture notes in computer science. Berlin, Heidelberg: Springer Berlin Heidelberg, pp. 347–360. Available at: http://dx.doi.org/10.1007/3540608052_77.

Singh, M.P., 2003. Agent communication languages: Rethinking the principles. In Communication in Multiagent Systems. Lecture notes in computer science. Berlin, Heidelberg: Springer Berlin Heidelberg, pp. 37–50. Available at: http://dx.doi.org/10.1007/978-3-540-44972-0_2.

Wooldridge, M. (2009) ‘An Introduction to Multi Agent Systems’. United Kingdom: John Wiley & Sons, Incorporated.