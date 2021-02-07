# Knowledge check

1. What is Durable Functions?

    - [x] TDurable Functions is an extension of Azure Functions, that allow you to simplify complex stateful executions in a serverless-environment
    - [ ] TDurable Functions is a logical container for a single workflow that you define using triggers and actions.
    - [ ] TDurable Functions is a serverless compute service that enables you to run code on-demand without having to explicitly provision or manage infrastructure.

Answer: Durable Functions is an extension of Azure Functions, that allow you to simplify complex stateful executions in a serverless-environment

2. Which of the following best describes the role of the Orchestrator function in a workflow?

    - [ ] It's used as the basic unit of work (actions and tasks) in a durable function orchestration.
    - [ ] It's the entry point for creating an instance of a Durable Functions orchestration.
    - [x] It's used for describing how actions are executed and the order in which actions are executed.

Answer: The Orchestrator Function is written in code. The function is used for describing how actions are executed and the order in which actions are executed.

3. Which of the following best explains why the Human Interaction application pattern benefits from Durable Functions?

    - [x] A manual process within an automated process because people aren't as highly available and as responsive as computers.
    - [ ] It addresses the problem of coordinating the state of long-running operations with external clients.
    - [ ] It allows the output from one function to be applied to input of the next function in a series of function calls.

Answer: Human interaction can be incorporated using timeouts and compensation logic.