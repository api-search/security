---
api_key_in: []
api_specs:
- filename: tensorwave-scalarlm-openapi.yml
  format: yaml
  label: ScalarLM API
  slug: scalarlm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorwave/refs/heads/main/openapi/tensorwave-scalarlm-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Tensorwave Authentication
name_suffix: Authentication
oauth_flows: []
overview: TensorWave declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: TensorWave
provider_slug: tensorwave
scheme_count: 0
schemes: []
slug: tensorwave-authentication
source_filename: tensorwave-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://www.scalarlm.com/inference/\nspec_source: openapi/tensorwave-scalarlm-openapi.yml\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: 'ScalarLM declares NO securitySchemes. This is a real finding, not a gap in the harvest:\n    the FastAPI application in tensorwavecloud/ScalarLM registers no authentication dependency on\n    any router, and the documented request examples on scalarlm.com send no credential of any\n    kind. A ScalarLM deployment is expected to be perimeter-protected by the operator (private\n    network, ingress auth, or an API gateway in front of it), not by the application.'\nschemes: []\ndocumented_examples:\n- source: https://www.scalarlm.com/inference/\n  request: |\n    curl https://gpt-oss.cray-lm.com/v1/chat/completions \\\n        -H \"Content-Type: application/json\" \\\n        -d '{\"messages\": [{\"role\": \"user\", \"content\": \"...\"}]}'\n  credentials: none\n- source:\
  \ https://www.scalarlm.com/inference/\n  request: |\n    import scalarlm\n    scalarlm.api_url = \"https://gpt-oss.cray-lm.com\"\n    llm = scalarlm.SupermassiveIntelligence()\n  credentials: none\n  note: The Python client is configured with a base URL only; it takes no API key.\ncredentials_in_payloads:\n- field: hf_token\n  operation: publishToHuggingFace\n  kind: third-party bearer token\n  description: 'A Hugging Face access token with write permission, supplied by the caller in the\n    PublishRequest body so ScalarLM can push a checkpoint to the Hub. It authenticates to Hugging\n    Face, not to ScalarLM.'\n  handling: 'Per the source docstring, the token is forwarded to sbatch via env-var export and is\n    never written to disk or argv on the API pod side.'\nplatform_authentication:\n  scope: The TensorWave GPU cloud platform (not the ScalarLM API)\n  model: 'Not an API. Access to bare-metal nodes, Slurm and Kubernetes is by SSH public key,\n    managed per user; team membership\
  \ and access are administered by org admins in the TensorWave\n    console.'\n  docs:\n  - https://docs.tensorwave.com/user-and-team-management/syncing-public-keys\n  - https://docs.tensorwave.com/user-and-team-management/managing-team-member-access\n  - https://docs.tensorwave.com/user-and-team-management/self-serve-inviting-users\n  - https://docs.tensorwave.com/slurm/access\n  mechanisms:\n  - ssh-public-key\n  - organization-role (admin vs member)\noauth2: false\noidc: false\nscopes_artifact: null\nscopes_note: No OAuth 2.0 surface exists, so no scopes/ artifact is emitted.\nrisks:\n- id: unauthenticated-write-operations\n  severity: high\n  detail: 'With no application-level auth, every operation in the derived spec is reachable by any\n    caller who can reach the deployment, including destructive ones: clearQueue,\n    cancelTrainingJob, restartTrainingJob, deleteTrainingJob, cancelSlurmJob and\n    publishToHuggingFace. Operators must not expose a ScalarLM deployment directly to\
  \ the public\n    internet.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensorwave/refs/heads/main/authentication/tensorwave-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Cloud Computing
- GPU
- Infrastructure
- Inference
- Model Training
- High Performance Computing
- Data Centers
---
