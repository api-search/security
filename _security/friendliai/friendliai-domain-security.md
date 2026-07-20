---
api_specs:
- filename: friendliai-openapi-original.yml
  format: yaml
  label: Friendli Suite API
  slug: friendli-suite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendliai/refs/heads/main/openapi/friendliai-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: friendli.ai
  spf: true
hosts:
- cert_expires: Sep 25 06:50:18 2026 GMT
  host: friendli.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.friendli.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Friendliai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FriendliAI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FriendliAI
provider_slug: friendliai
slug: friendliai-domain-security
source_filename: friendliai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: friendli.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:50:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.friendli.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: friendli.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friendliai/refs/heads/main/security/friendliai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Artificial Intelligence
- Machine Learning
- LLM
- Inference
- Generative AI
- GPU
- OpenAI Compatible
---
