# DSC 180A Methodology Assignment 4

**Name:** Jiahe Qin  
**Email:** [jiq004@ucsd.edu](mailto:jiq004@ucsd.edu)

**Section:** D30, Steering Large Language Models  
**Mentors:** Tianhao Wang and Misha Belkin

---

**1. What is the most interesting topic covered in your domain this quarter?**

The most interesting topic has been the tension between steering a model toward a desired behavior while keeping its general reasoning ability. Methods that we saw in discussion can make a model behave more willingly in a certain way, but an intervention aimed at one behavior can hurt its ability to be intelligent. I find it interesting that "does the model abstain?" and "does the model abstain for the right reasons?" are different questions, and that answering the second one requires careful measurement.

**2. Describe a potential investigation you would like to pursue for your Quarter 2 Project.**

I would like to study whether steering a model's internal representations toward uncertainty or honesty can improve abstention without lowering accuracy on questions the model can answer. Concretely, I would like to compare a few steering approaches on question-answering and reasoning benchmarks. I would measure both calibration and selective prediction quality, and check how much each approach influences reasoning performance.

**3. What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**

What my team is focusing on now in Quarter 1 is replication. For the most part, I think the approach is trivial and there is no cutting corners. If any changes were to be made, it has to be how efficient we are at reading the papers. Whether it's leveraging AI for understanding or for computational support, it can speed us up.

**4. What other techniques would you be interested in using in your project?**

Something I would be interested in is trying preference-based methods to compare against activation steering, and uncertainty estimation methods such as sampling-based consistency checks and verbalized confidence. I would also like to try probing the model's hidden states with simple linear classifiers to see whether an uncertainty direction exists before attempting to steer along it.
