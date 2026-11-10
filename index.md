# DSC 180A Methodology Assignment 4

**Name:** Jiahe Qin
**Email:** [jiq004@ucsd.edu](mailto:jiq004@ucsd.edu)

**Section:** D30, Steering Large Language Models
**Mentors:** Tianhao Wang and Misha Belkin

---

**1. What is the most interesting topic covered in your domain this quarter?**

The most interesting topic has been the tension between steering a model toward a desired behavior and keeping its general reasoning ability. Methods such as prompting, fine-tuning, preference optimization and activation steering can make a model more calibrated or more willing to say "I don't know," but an intervention aimed at one behavior can quietly hurt another, such as math reasoning. I find it interesting that "does the model abstain?" and "does the model abstain for the right reasons?" are different questions, and that answering the second one requires careful measurement.

**2. Describe a potential investigation you would like to pursue for your Quarter 2 Project.**

I would like to study whether steering a model's internal representations toward uncertainty or honesty can improve abstention without lowering accuracy on questions the model can answer. Concretely, I would compare a few steering approaches (activation steering and a fine-tuned baseline) on question-answering and reasoning benchmarks. I would measure both calibration (for example, expected calibration error) and selective prediction quality (accuracy at a given coverage), and check how much each approach degrades reasoning performance.

**3. What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**

I would evaluate on a wider and more varied set of tasks and models instead of relying on a small number of benchmarks. Results that look good on one dataset can fail to carry over to another, so testing across several would make the conclusions more trustworthy. I would also report uncertainty in my results, such as confidence intervals over multiple random seeds, rather than single-run numbers.

**4. What other techniques would you be interested in using in your project?**

I would be interested in trying preference-based methods (RLHF-style or direct preference optimization) to compare against activation steering, and uncertainty estimation methods such as sampling-based consistency checks and verbalized confidence. I would also like to try probing the model's hidden states with simple linear classifiers to see whether an "uncertainty direction" exists before attempting to steer along it.
