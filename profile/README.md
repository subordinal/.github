<p align="center">
  <img src="banner.png" alt="Subordinal. Model readiness for self-hosted inference." width="100%">
</p>

## Model readiness for self-hosted inference

Large models take minutes to start, and sometimes they do not start at all. Subordinal tells an ML platform team, before and during a rollout:

- **Will it start?** Model, runtime, quantization and GPU checked against each other.
- **How long until ready?** Startup split into fetch, weight load, compile and init.
- **Why is it slow or failing?** One diagnosis across storage, cache, runtime and Kubernetes.
- **What fixes it?** A concrete change, and the GPU cost of the time spent not serving.

Vendor neutral, across vLLM, SGLang, KServe and Kubernetes. Open source first.

## readyml

[readyml](https://github.com/subordinal/readyml) is the open-source CLI. It downloads no weights and needs no GPU.

- `readyml check`: a model against a vLLM or SGLang release and a GPU type.
- `readyml versions`: which releases load a model's architecture.
- `readyml trace`: where startup time went, from a server log.

Website: [subordinal.github.io](https://subordinal.github.io)

**Status:** early development.
