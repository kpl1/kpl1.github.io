# Vision

## What is a QA Engineer ?

- He doesn't participate in code creation for the product, so he doesn't create quality.
- He found the truth about the current state of the product and give the alert to the team.
- He is not the last line of defense.
- Agility, pragmatism and team spirit



```mermaid
graph LR
    create ---> AutomatedTesting
    maintain ---> AutomatedTesting
    testData ---> AutomatedTesting
    AutomatedTesting <---> QualityAssurance
    QualityAssurance<-->A[fa:fa-spinner ManualTesting]
    QualityAssurance<-->B(fa:fa-spinner QualityAssitance)
    A[fa:fa-spinner ManualTesting] ---> PairTesting
    A[fa:fa-spinner ManualTesting] --->  Investigation
    A[fa:fa-spinner ManualTesting] --->  Exploration
    A[fa:fa-spinner ManualTesting] --->  TestPlanification
    B[fa:fa-spinner QualityAssitance] ---> AdvocateForQuality
    B[fa:fa-spinner QualityAssitance] ---> ShareProductKnowledge
    B[fa:fa-spinner QualityAssitance] ---> EvaluateIssue
    B[fa:fa-spinner QualityAssitance] ---> Specification
    B[fa:fa-spinner QualityAssitance] ---> Documentation
```


## What is quality ? 

- It's the confidence on a working product delivered in production. 



