---
api_specs:
- filename: kataai-auth-api-openapi.yml
  format: yaml
  label: Kata.ai Auth API
  slug: kataai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-auth-api-openapi.yml
- filename: kataai-bots-api-openapi.yml
  format: yaml
  label: Kata.ai Bots API
  slug: kataai-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-bots-api-openapi.yml
- filename: kataai-channels-api-openapi.yml
  format: yaml
  label: Kata.ai Channels API
  slug: kataai-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-channels-api-openapi.yml
- filename: kataai-deployments-api-openapi.yml
  format: yaml
  label: Kata.ai Deployments API
  slug: kataai-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-deployments-api-openapi.yml
- filename: kataai-environments-api-openapi.yml
  format: yaml
  label: Kata.ai Environments API
  slug: kataai-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-environments-api-openapi.yml
- filename: kataai-nlu-api-openapi.yml
  format: yaml
  label: Kata.ai NLU API
  slug: kataai-nlu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-nlu-api-openapi.yml
- filename: kataai-prediction-api-openapi.yml
  format: yaml
  label: Kata.ai Prediction API
  slug: kataai-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-prediction-api-openapi.yml
- filename: kataai-projects-api-openapi.yml
  format: yaml
  label: Kata.ai Projects API
  slug: kataai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-projects-api-openapi.yml
- filename: kataai-teams-api-openapi.yml
  format: yaml
  label: Kata.ai Teams API
  slug: kataai-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/openapi/kataai-teams-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "usertrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kata.ai
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: kata.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 15:44:15 2026 GMT
  host: docs.kata.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 02:17:04 2026 GMT
  host: api.kata.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kataai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kata.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kata.ai
provider_slug: kataai
slug: kataai-domain-security
source_filename: kataai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: null\n- host: docs.kata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:44:15 2026 GMT\n  hsts: null\n- host: api.kata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 02:17:04 2026 GMT\n  hsts: null\ndomains:\n- domain: kata.ai\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"usertrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kataai/refs/heads/main/security/kataai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Conversational AI
- Chatbots
- AI Agents
- Natural Language Understanding
- NLU
- Customer Experience
- Messaging
- Indonesia
- Bots
---
