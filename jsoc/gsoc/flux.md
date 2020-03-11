#  Machine Learning Projects - Summer of Code

### CUDA Hacking

Are you a performance nut? Help us implement cutting-edge CUDA kernels in Julia for operations important across deep learning, scientific computing and more. We also need help developing our wrappers for machine learning, sparse matrices and more, as well as CI and infrastructure. Contact us to develop a project plan.

Mentors: [Tim Besard](https://github.com/maleadt), [Mike Innes](https://github.com/MikeInnes).

### Reinforcement Learning Environments

Develop a series of reinforcement learning environments, in the spirit of the [OpenAI Gym](https://gym.openai.com). Although we have wrappers for the gym available, it is hard to install (due to the Python dependency) and, since it's written in Python and C code, we can't do more interesting things with it (such as differentiate through the environments). A pure-Julia version that supports a similar API and visualisation options would be valuable to anyone doing RL with Flux.

Mentors: [Dhairya Gandhi](https://github.com/dhairyagandhi96/).

### NLP Tools and Models

Build deep learning models for Natural Language Processing in Julia. [TextAnalysis](https://github.com/juliatext/TextAnalysis.jl)  and [WordTokenizers](https://github.com/JuliaText/WordTokenizers.jl) contains the basic algorithms and data structures to work with textual data in Julia. On top of that base, we want to build modern deep learning models based on recent research. The following tasks can span multiple students and projects.

It is important to note that we want practical, usable solutions to be created, not just research models. This implies that a large part of the effort will need to be in finding and using training data, and testing the models over a wide variety of domains. Pre-trained models must be available to users, who should be able to start using these without supplying their own training data.

* Implement [ELMo](https://allennlp.org/elmo) in Julia
* Implement [ALBERT](https://ai.googleblog.com/2019/12/albert-lite-bert-for-self-supervised.html) in Julia
* Implement GPT/GPT-2 in Julia
* Implement [extractive summarisation based on Transformers](https://arxiv.org/abs/1909.03186)
* Implement practical models for
  * Dependency Tree Parsing  
  * Morphological extractions  
  * Translations (using Transformers)  
* Indic language support -- validate and test all models for Indic languages
  * ULMFiT models for Indic languages
* Chinese tokenisation and parsing

**Mentors**: [Avik Sengupta](https://github.com/aviks/)

### Automated music generation

Neural network based models can be used for music analysis and music generation (composition). A suite
of tools in Julia to enable research in this area would be useful. This is a large, complex project that
is suited for someone with an interest in music and machine learning. This project will need a mechanism
to read music files (primarily MIDI), a way to synthesise sounds, and finally a model to learn composition.
All of this is admittedly a lot of work, so the exact boundaries of the project can be flexible, but this can be an
exciting project if you are interested in both music and machine learning.

**Recommended Skills**: Music notation, some basic music theory, MIDI format, Transformer and LSTM architectures

**Resources**: [Music Transformer](https://magenta.tensorflow.org/music-transformer), [Wave2MIDI2Wave](https://magenta.tensorflow.org/maestro-wave2midi2wave)

**Mentors**: [Avik Sengupta](https://github.com/aviks/)

## Flux.jl

Flux usually takes part in [Google Summer of Code](https://summerofcode.withgoogle.com), as part of the wider Julia organisation. We follow the same [rules and application guidelines](https://julialang.org/soc/ideas-page) as Julia, so please check there for more information on applying. Below are a set of ideas for potential projects (though you are welcome to explore anything you are interested in).

Flux projects are typically very competitive; we encourage you to get started early, as successful students typically have early PRs or working prototypes as part of the application. It is a good idea to simply start contributing via issue discussion and PRs and let a project grow from there; you can take a look at [this list of issues](https://github.com/issues?utf8=✓&q=is%3Aopen+archived%3Afalse+user%3AFluxML+label%3A%22help+wanted%22) for some starter contributions.

### Port ML Tutorials

There are many high-quality open-source tutorials and learning materials available, for example from PyTorch and fast.ai. We'd like to have Flux ports of these that we can add to the model zoo, and eventually publish to the Flux website.

Mentors: [Dhairya Gandhi](https://github.com/dhairyagandhi96/).

### Model Zoo Examples

Flux's [model zoo](https://github.com/FluxML/model-zoo/) contains examples of a wide range of deep learning models and techniques. This project would involve adding new models, showing how to recreate state-of-the-art results (e.g. AlphaGo) or interesting and unusual model architectures (e.g. transformer networks). We'd be particularly interested in any models involving reinforcement learning, or anything with images, sound or speech.

Some experience with implementing deep learning models would be ideal for this project, but is not essential for a student willing to pick up the skills and read ML papers. It's up to you whether you implement a single ambitious model, or multiple small ones. A good source of inspiration might be the [NIPS Challenge](https://nurture.ai/nips-challenge).

*Note that this project is quite popular; students who show skills and interests in other parts of the stack may have an easier time distinguishing themselves.*

Mentors: [Dhairya Gandhi](https://github.com/dhairyagandhi96/).

## Deep Learning for 3D Computer Vision

Build deep learning models for 3D computer vision using Flux. There has been a lot of interest in exploiting 3D models (in the form of Voxels, Point Clouds, Meshes, etc.) for developing more reliable computer vision models. The objective of this project would be to develop a framework (powered by Flux + Zygote) which helps accelerate 3D Computer Vision research in Julia.

Some inspiration could be drawn from python frameworks like [Kaolin](https://kaolin.readthedocs.io/en/latest/), [Pytorch3D](https://pytorch3d.readthedocs.io/en/latest/overview.html), and [Tensorflow Graphics](https://www.tensorflow.org/graphics/overview). This project would involve developing (a few of) the following modules:

@@tight-list
* Integration with Differentiable Graphics Frameworks (like [RayTracer.jl](https://github.com/avik-pal/RayTracer.jl) or bindings with non-Julia ones like [DiB-R](https://nv-tlabs.github.io/DIB-R/) and [Soft Rasterizer](http://vgl.ict.usc.edu/Research/softrasterizer/).
* Graphics engine for (differentiable) interconversion across various representations like Voxels, Point Clouds, SDFs, Meshes, etc.
* Deep Learning Models like PointCNN, DGCNN, PointCNN++, etc or other newer models.
* Examples using these components for 3D Reconstruction, Object Synthesis using GANs, 3D Object Tracking, etc.
* Integration with Graph Neural Network framework (https://github.com/yuehhua/GeometricFlux.jl).
@@

**Recommended Skills:** Should be familiar with 2D Computer Vision, but knowledge of 3D vision would be preferable. Some background with computer graphics would be desirable.

**Expected Outcome:** A 3D Computer Vision Framework for future research using Flux.

**Mentors:** [Avik Pal](https://avik-pal.github.io), [Elliot Saba](https://github.com/staticfloat)
