---
api_key_in: []
api_specs:
- filename: evolutionaryscale-embeddings-api-openapi.yml
  format: yaml
  label: EvolutionaryScale Embeddings API
  slug: evolutionaryscale-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/openapi/evolutionaryscale-embeddings-api-openapi.yml
- filename: evolutionaryscale-encoding-api-openapi.yml
  format: yaml
  label: EvolutionaryScale Encoding API
  slug: evolutionaryscale-encoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/openapi/evolutionaryscale-encoding-api-openapi.yml
- filename: evolutionaryscale-generation-api-openapi.yml
  format: yaml
  label: EvolutionaryScale Generation API
  slug: evolutionaryscale-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/openapi/evolutionaryscale-generation-api-openapi.yml
- filename: evolutionaryscale-msa-api-openapi.yml
  format: yaml
  label: EvolutionaryScale MSA API
  slug: evolutionaryscale-msa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/openapi/evolutionaryscale-msa-api-openapi.yml
- filename: evolutionaryscale-sampling-api-openapi.yml
  format: yaml
  label: EvolutionaryScale Sampling API
  slug: evolutionaryscale-sampling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/openapi/evolutionaryscale-sampling-api-openapi.yml
- filename: evolutionaryscale-structure-api-openapi.yml
  format: yaml
  label: EvolutionaryScale Structure API
  slug: evolutionaryscale-structure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/openapi/evolutionaryscale-structure-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Evolutionaryscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: EvolutionaryScale secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EvolutionaryScale
provider_slug: evolutionaryscale
scheme_count: 1
schemes:
- description: Forge API token issued via forge.evolutionaryscale.ai.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/evolutionaryscale-forge-esm3-api-openapi.yml
  - openapi/evolutionaryscale-forge-esmc-api-openapi.yml
  - openapi/evolutionaryscale-forge-folding-api-openapi.yml
  type: http
slug: evolutionaryscale-authentication
source_filename: evolutionaryscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/evolutionaryscale-forge-esm3-api-openapi.yml, openapi/evolutionaryscale-forge-esmc-api-openapi.yml,\n  openapi/evolutionaryscale-forge-folding-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Forge API token issued via forge.evolutionaryscale.ai.\n  sources:\n  - openapi/evolutionaryscale-forge-esm3-api-openapi.yml\n  - openapi/evolutionaryscale-forge-esmc-api-openapi.yml\n  - openapi/evolutionaryscale-forge-folding-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/authentication/evolutionaryscale-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Biology
- Bioinformatics
- Computational Biology
- Drug Discovery
- ESM
- ESM3
- ESM Cambrian
- Foundation Models
- Generative Biology
- Life Sciences
- Machine-Learning
- Protein Design
- Protein Folding
- Protein Language Models
- Proteins
- Representation Learning
- Structure Prediction
---
