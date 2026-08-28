---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Free Exercise Db Authentication
name_suffix: Authentication
oauth_flows: []
overview: Free Exercise DB declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Free Exercise DB
provider_slug: free-exercise-db
scheme_count: 0
schemes: []
slug: free-exercise-db-authentication
source_filename: free-exercise-db-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://github.com/yuhonas/free-exercise-db#how-do-i-use-them\ndocs: https://github.com/yuhonas/free-exercise-db#how-do-i-use-them\nname: Free Exercise DB Authentication\nsummary: >-\n  No authentication of any kind. The provider's README documents consumption as a plain\n  HTTPS GET against raw.githubusercontent.com — no account, no key, no token, no\n  registration step exists anywhere in the project. This is the complete auth profile,\n  not a gap in our research: there is nothing to authenticate to.\nauth_required: false\nsecurity_schemes: []\nschemes_observed:\n- style: none\n  transport: https\n  note: >-\n    Verified by an anonymous GET of dist/exercises.json (HTTP 200, 1,001,472 bytes) with\n    no Authorization header.\nnotes:\n- >-\n    Because the dataset is served from GitHub's raw content CDN, GitHub's own anonymous\n    access rules apply to the transport. The provider publishes no auth layer of its own\n   \
  \ and issues no credentials.\n- >-\n    No OAuth, no OpenID Connect, no API keys, no mTLS — scopes/ is therefore not\n    applicable and no scopes artifact is written.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/free-exercise-db/refs/heads/main/authentication/free-exercise-db-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Open Data
- Fitness
- Exercise
- Health
- Public Domain
- Dataset
- JSON Schema
- Workout
---
