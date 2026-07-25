---
api_specs:
- filename: inception-labs-chat-api-openapi.yml
  format: yaml
  label: Inception Labs Chat API
  slug: inception-labs-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inception-labs/refs/heads/main/openapi/inception-labs-chat-api-openapi.yml
- filename: inception-labs-edit-api-openapi.yml
  format: yaml
  label: Inception Labs Edit API
  slug: inception-labs-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inception-labs/refs/heads/main/openapi/inception-labs-edit-api-openapi.yml
- filename: inception-labs-fim-api-openapi.yml
  format: yaml
  label: Inception Labs FIM API
  slug: inception-labs-fim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inception-labs/refs/heads/main/openapi/inception-labs-fim-api-openapi.yml
- filename: inception-labs-models-api-openapi.yml
  format: yaml
  label: Inception Labs Models API
  slug: inception-labs-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inception-labs/refs/heads/main/openapi/inception-labs-models-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: inceptionlabs.ai
  spf: true
hosts:
- cert_expires: Aug 21 11:19:33 2026 GMT
  host: inceptionlabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: api.inceptionlabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inception Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inception Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Inception Labs
provider_slug: inception-labs
slug: inception-labs-domain-security
source_filename: inception-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inceptionlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:19:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.inceptionlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: inceptionlabs.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inception-labs/refs/heads/main/security/inception-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Diffusion Models
- Generative AI
- Code Completion
- LLM API
- OpenAI Compatible
- Developer Tools
- Company
---
