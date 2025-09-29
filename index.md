---
layout: page
homepage: True
title: Home
---

{: style="margin-top: 0.5rem; margin-bottom: 0;"}
# Stopping Agents

{: style="margin-top: 0.25rem;"}
*Language agents for optimal stopping*

{: style="margin-top: 1.8rem;"}
Stopping agents are language agents --- large language models that
generate *decisions* --- specialized for optimal stopping of conversations.

Specifically, stopping agents observe the ongoing conversation text and
make sequential `wait` or `quit` decisions that optimally tradeoff between waiting
to accumulate more information and incurring waiting costs.

This software implements the algorithm proposed in [our paper](#):

{: style="color: #666; font-size: 0.7em; "}
> Manzoor, Emaad, and Ascarza, Eva and Netzer, Oded. "Learning When to Quit in Sales Conversations." arXiv preprint arXiv:????.????? (2025).

![demo](images/demo.gif)
Check out our demo [on Github](https://github.com/emaadmanzoor/stopping-agents/)!
{:.caption}

<hr/>
