---
layout: page
permalink: /examples/
title: Examples
---

{: style="margin-top: 0.5rem; margin-bottom: 0;"}
# Stopping Agents

{: style="margin-top: 0.25rem;"}
*Language agents for optimal stopping*

## Example: Behavioral Cloning

The example Python code below trains a behavioral cloning agent on a dataset
of sales conversations.

```python
from stopping_agents.env import SalesCallEnv
from stopping_agents.behavioral_cloning import BehavioralCloningAgent

# Initialize the environment with your dataset and parameters
env = SalesCallEnv(
    dataset=your_dataset,
    time_checkpoints=[60, 90],
    cost_per_second=0.0025,
    benefit_per_sale=1.0
)

# Create and train the agent
agent = BehavioralCloningAgent(env.action_space)
agent.train(your_dataset)

# Evaluate the agent
obs, _ = env.reset()
done = False
while not done:
    action = agent.predict(obs)
    obs, reward, done, _, _ = env.step(action)
```
