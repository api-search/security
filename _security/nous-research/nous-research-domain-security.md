---
api_specs:
- filename: nous-research-inference-api-openapi.yml
  format: yaml
  label: Nous Research Inference API (Nous Portal)
  slug: nous-research-inference-api-nous-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nous-research/refs/heads/main/openapi/nous-research-inference-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nousresearch.com
  spf: true
hosts:
- cert_expires: Aug 29 20:25:40 2026 GMT
  host: nousresearch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 09:30:06 2026 GMT
  host: portal.nousresearch.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 09:40:16 2026 GMT
  host: inference-api.nousresearch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nous Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nous Research, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nous Research
provider_slug: nous-research
slug: nous-research-domain-security
source_filename: nous-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nousresearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:25:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.nousresearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:30:06 2026 GMT\n  hsts: null\n- host: inference-api.nousresearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 09:40:16 2026 GMT\n  hsts: false\ndomains:\n- domain: nousresearch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nous-research/refs/heads/main/security/nous-research-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Machine Learning
- Large Language Models
- Inference
- Agents
- Open Weights
- x402
---
