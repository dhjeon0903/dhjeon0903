## Dong Hyeon Jeon

B.S. Data Science, University of Wisconsin–Madison (Dec 2026).
I work on verification in production data systems: the gap between what a
system reports about itself and what is actually true of it.

### Preprints

**Silent Success: A Release Gate That Passed on Checks It Never Ran, and Eight More**
[arXiv:2609.30307](https://arxiv.org/abs/2609.30307) · 27 pp.
Nine cases where a description of a system was used as evidence for its state.
Seven of the nine would have been caught by a single query, command, or
comparison. Derives a three-valued verdict (pass / violation / unable to
determine) that turns a silent pass into a failure.

**Empty Intersection: Provenance Coverage Rose to 98% and Neither Verification Decision Moved**
[arXiv:2609.30308](https://arxiv.org/abs/2609.30308) · 12 pp.
Two standard provenance remedies measured against a frozen snapshot of 194,620
rows. Coverage rose from 36.0980% to 98.4226%. The rows the interventions
repaired and the 32 rows the decisions read do not intersect. A null result.

### Upstream contributions

Three defects of the same shape, found in projects I did not write, patched
upstream. All three appear as cases in the first preprint.

| Project | PR | Defect |
|---|---|---|
| [vLLM](https://github.com/vllm-project/vllm/pull/51228) | #51228 | Repeated encoder-cache slot releases pushed `num_free_slots` past `cache_size`, invalidating the admission constraint |
| [LiteLLM](https://github.com/BerriAI/litellm/pull/35934) | #35934 | `default_redis_ttl` was never applied to Redis write paths, so the effective TTL diverged from the declared configuration |
| [MLflow](https://github.com/mlflow/mlflow/pull/24953) | #24953 | Batches merged into one failing backend operation reported success to child callers |

### Now

System Architect at HAE-ai, building an agentic digital twin platform for
industrial process monitoring. The hard part is not the model: it is data
provenance, permission boundaries between agents, approval gates, and
evaluation that actually fails when it should.

### Links

[Portfolio](https://dhjeon0903.github.io/Dong-Hyeon-Jeon) · djeon4@wisc.edu
