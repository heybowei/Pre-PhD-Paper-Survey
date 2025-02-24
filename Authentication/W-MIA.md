# W-MIA Membership Inference Attack against Deep Learning-based RF Fingerprinting

[Paper Link](https://ieeexplore.ieee.org/document/10735522)

**Background:** Deep learning-base RF fingerprint (DRFF) is a way to authenicate devices based on the fact that every devices have unique charactoristics, e.g. hardware imperfection, amplification...

## STAR Principle

**Situation and Tasks:** A verifier and many verified devices are in the picture. It wants to launch an attack that is not veried before but still can pass the authentication.

**Actions:** It places a monitor near the verifier to get the authenticated RF samples, saved in the dataset. And tune it by generating impersonated while not legal RF samples.

## How does this paper can be used to me

1. It uses simulated and existing dataset.

2. Sample generation method: newton method.