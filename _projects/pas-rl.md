---
title: Probably Approximate Safe RL Policy
image: '/images/projects/pas_rl/safeai.jpeg'
---


With the advancement of machine learning based automation in the current digital world, the problem of safety verification of such systems is becoming crucial, especially in safety-critical domains like self-driving cars, robotics, etc. Reinforcement learning (RL) is an emerging machine learning technique with many applications, including in safety-critical domains. The classical safety verification approach of making a binary decision on determining whether a system is safe or unsafe is particularly challenging for an RL system. Such an approach generally requires prior knowledge about the system, e.g., the transition model of the system, the set of unsafe states in the environment, etc., which are typically unavailable in a standard RL setting. Instead, this paper addresses the safety verification problem from a quantitative safety perspective, i.e., we quantify the safe behavior of the policy in terms of probability. We formulate the safety verification problem as a chance-constrained optimization using the technique of barrier certificate. We then use a sampling based approach called scenario optimization to solve the chance-constrained problem, which gives the desired probabilistic guarantee on the safe behavior of the policy. Our extensive empirical evaluation shows the validity and robustness of our approach in three RL domains.

<font size=4><a href="https://www.ifaamas.org/Proceedings/aamas2024/pdfs/p1745.pdf">[Paper: AAMAS-2024]</a></font>

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/projects/pas_rl/arch.png" alt="Project">    
  </div>
  <em>The figure shows the system diagram of our proposed probably approximate safety (PAS) verification approach. The trajectory samples of the policy 𝜋 test are obtained from the simulator. Like the reward value, the simulator also provides a cost value 𝑐_𝑡 at each time step, which is used to compute the safety value of trajectory 𝑉_unsafe(𝜏). For given values of the safety threshold 𝛼 and confidence level (1 − 𝛽), our PAS verification approach provides the barrier region (C_B𝜙 ) along with the probability of safe behavior (1 − 𝜖) of the policy.</em>
</div>

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/projects/pas_rl/pas_rl.png" alt="Project">
  </div>
  <em>The figures show an approximate graphical representation of the barrier region of the unsafe and safe policies for the safe navigation environment. The green polygon denotes the barrier region with trajectory samples inside it.</em>
</div>
