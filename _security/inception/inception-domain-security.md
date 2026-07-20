---
api_specs:
- filename: inception-openapi-original.json
  format: json
  label: Inception API
  slug: inception-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inception/refs/heads/main/openapi/inception-openapi-original.json
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
name: Inception Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inception, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Inception
provider_slug: inception
slug: inception-domain-security
source_filename: inception-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inceptionlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:19:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.inceptionlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: inceptionlabs.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inception/refs/heads/main/security/inception-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai Ml
- LLM
- Artificial Intelligence
- Diffusion Models
- Code Completion
- Machine Learning
- Developer Tools
---
