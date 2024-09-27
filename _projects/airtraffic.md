---
title: Air Traffic Control
image: '/images/airtraffic.jpg'
---

Many real world systems involve interaction among large number of agents to achieve a common goal, for example, air traffic control. Several model-free RL algorithms have been proposed for such settings. A key limitation is that the empirical reward signal in model-free case is not very effective in addressing the multiagent credit assignment problem, which determines an agent's contribution to the team's success. This results in lower solution quality and high sample complexity. To address this, we contribute (a) an approach to learn a differentiable reward model for both continuous and discrete action setting by exploiting the collective nature of interactions among agents, a feature commonly present in large scale multiagent applications; (b) a shaped reward model analytically derived from the learned reward model to address the key challenge of credit assignment; (c) a model-based multiagent RL approach that integrates shaped rewards into well known RL algorithms such as policy gradient, soft-actor critic. Compared to previous methods, our learned reward models are more accurate, and our approaches achieve better solution quality on synthetic and real world instances of  air traffic control, and cooperative navigation with large agent population.

<font size=4><a href="https://jamesarambam.github.io/files/icaps21.pdf">[Paper: ICAPS-2021]</a></font>

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/projects/london3.png" alt="Project">
  </div>
  <em>Figure shows an air traffic scenario over London Heathrow Airport</em>
</div>
