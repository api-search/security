---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DeepMind Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeepMind declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DeepMind
provider_slug: deepmind
scheme_count: 1
schemes:
- applies_to: AlphaGenome API (gdmscience.googleapis.com:443, gRPC over TLS)
  evidence: 'create(api_key, address=None): metadata=[(''x-goog-api-key'', api_key)], address default ''dns:///gdmscience.googleapis.com:443'''
  in: header (gRPC metadata)
  name: AlphaGenome API key
  parameter: x-goog-api-key
  type: apiKey
slug: deepmind-authentication
source_filename: deepmind-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: DeepMind authentication\ngenerated: '2026-11-12'\nmethod: searched\nsource: https://github.com/google-deepmind/alphagenome/blob/main/src/alphagenome/models/v1/dna_client.py\ndocs: https://alphagenome.google/api\nschemes:\n- name: AlphaGenome API key\n  type: apiKey\n  in: header (gRPC metadata)\n  parameter: x-goog-api-key\n  applies_to: AlphaGenome API (gdmscience.googleapis.com:443, gRPC over TLS)\n  evidence: 'create(api_key, address=None): metadata=[(''x-goog-api-key'', api_key)], address default ''dns:///gdmscience.googleapis.com:443'''\nnote: Gemini/Gemma model access is authenticated by Google AI Studio API keys and is profiled under the google-gemini\n  provider.\n"
source_yaml_url: https://artifacts.apis.io/deepmind/authentication/deepmind-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Foundation Models
- LLM
- Research
- Robotics
- Developer Tools
---
