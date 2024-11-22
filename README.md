# LLM-Unlearning-for-Privacy-Information
This repository is dedicated to exploring **LLM unlearning**, focusing on privacy risks and strategies to effectively and efficiently "forget" specific data from large language models. 

---

## Key Topics

### Privacy Attack
- **Membership Inference Attacks (MIA):** Identifying training data.
- **Data Reconstruction Attacks:** Extracting sensitive content.
- **Privacy Regulation Compliance:** Addressing data deletion requests (e.g., GDPR).

---

## Unlearning Techniques

This section categorizes and summarizes the key techniques in unlearning, including **Parameter Optimization Method**, **Parameter Merging Method**, and **Parameter Agnostic Method**. Each technique is described alongside its key methods and referenced works.

---

### Parameter Optimization Method
Parameter optimization involves modifying model parameters to effectively "forget" specific data while maintaining the utility of the remaining model. This category includes gradient-based methods, second-order optimization, and general frameworks.

- **Who’s Harry Potter? Approximate Unlearning in LLMs**  
  - **Description:** Fine-tunes models to erase specific knowledge by swapping unique phrases with generalized alternatives.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2310.02238)

- **Partitioned Contrastive Gradient Unlearning (PCGU)**  
  - **Description:** Uses first-order gradient approximations to refine weights and efficiently remove biases.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2311.07568)
 
- **Knowledge unlearning for mitigating privacy risks in language models**  
  - **Description:** Uses gradient ascent for unlearning and propose how to evaluate privacy protection of unlearning method
  - **Reference:** [Paper Link](https://arxiv.org/abs/2210.01504)

- **Negative Preference Optimization: From Catastrophic Collapse to Effective Unlearning**  
  - **Description:** Introduces a preference optimization framework to prevent catastrophic collapse during gradient ascent-based unlearning.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2404.05868)

- **Second-Order Information Matters**  
  - **Description:** Employs Hessian-based methods for precise parameter adjustments to ensure privacy protection.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2403.10557)

- **KGA: A General Machine Unlearning Framework**  
  - **Description:** Aligns distribution gaps between learned and unlearned data, effectively applied to various NLP tasks.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2305.06535)

- **Towards Safer Large Language Models Through Machine Unlearning**  
  - **Description:** Introduces metrics like forget, mismatch, and maintain to optimize unlearning while balancing generalization and utility.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2402.10058)

- **DEPN: Detecting and Editing Privacy Neurons in Pretrained Language Models**  
  - **Description:** Detects and deactivates neurons associated with private information to perform unlearning.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2310.20138)

---

### Parameter Merging Method
Parameter merging focuses on reducing computational costs by applying arithmetic operations or selectively pruning model components.

#### Task Vectors
- **Editing Models with Task Arithmetic**  
  - **Description:** Introduced task vectors to define trajectories in weight space for flexible model alterations, including unlearning.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2203.13124)

#### Linear Arithmetic Operations
- **Composing Parameter-Efficient Modules with Arithmetic Operations**  
  - **Description:** Uses linear arithmetic operations like addition and negation to integrate parameter-efficient modules without retraining.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2403.02124)

#### Selective Neuron Pruning
- **Dissecting Language Models: Machine Unlearning via Selective Pruning**  
  - **Description:** Identifies and removes neurons related to specific behaviors, maintaining network efficiency.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2403.01267)

---

### Parameter Agnostic Method
It focuses on prompt-based methods to guide the model towards forgetting sensitive data dynamically.

- **In-Context Unlearning for LLMs**  
  - **Description:** Uses unlearning samples as prompts to adjust the model's outputs without modifying internal parameters.  
  - **Advantages:**  
    - Reduces computational costs.  
    - Suitable for real-time or on-demand unlearning.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2310.07579)

---

## Existing Unlearning Evaluation Framework

- **TOFU: Task of Fictitious Unlearning**  
  - **Description:** Uses a dataset of synthetic author profiles to benchmark unlearning techniques. Fine-tuning and KL-divergence metrics are applied for diverse datasets.  
  - **Reference:** [Paper Link](https://arxiv.org/abs/2401.06121)

---

## Future Directions
- Developing faster and more effective unlearning algorithms.
- Establishing standard benchmarks for unlearning evaluation.
