# Sutton and Barto Notebooks

## Rationale

The book [Reinforcement Learning: An Introduction](http://incompleteideas.net/book/the-book-2nd.html) is a great book for beginners to learn Reinforcement Learning. It contains clear descriptions and numerous examples and figures to clarify important concepts. The figures are a vital component of the book, so this repository aims to reproduce and explain the figures on the book with Python 3.

Sutton과 Barto가 쓴 [Reinforcement Learning: An Introduction](http://incompleteideas.net/book/the-book-2nd.html) 는 강화학습을 시작하시는 분들에게 정말 좋은 책입니다. 이 책은 중요한 개념들을 예제와 그림으로 명확하게 설명합니다. 이런 예제들과 그림들은 강화학습을 이해하는 데 굉장히 중요함으로, Python 3으로 책의 예제들을 구현하고 결과들을 재현하려고 합니다.

## Format

Most notebooks will consist of 3 parts: Environment, Agent(s), and Plot(s).

### Environment

The **Environment** section will have a Environment class. The Environment class will generally have these elements:

Variables

 * **action_space**: A list of all possible actions in the environment.
 * **state_space**: A list of all possible states in the environment.
 * **state**: Current state in the environment.

Methods

 * **step**: Takes a step with given action and return (next_state, reward, done, info)
 * **reset**: Resets the environment and returns the initial state.

### Agent

The **Agent** section will have the agent that can interact with the environment. The Agent class will generally have these elements:

Variables

 * **name**: A string that acts as a name of the agent.

Methods

 * **get_action**: Get action based on the agent's policy.
 * **update**: Update parameters based on (state, action, next_state, reward, done).
 * **reset**: Resets the agent back to initial values, before interacting with the environment.

### Plot

The **Plot** section will have the plots that resemble the figures in the book.
