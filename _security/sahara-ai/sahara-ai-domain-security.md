---
api_specs:
- filename: sahara-ai-compute-openapi.yml
  format: yaml
  label: Sahara AI Compute API
  slug: sahara-ai-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sahara-ai/refs/heads/main/openapi/sahara-ai-compute-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saharaai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: saharalabs.ai
  spf: true
hosts:
- cert_expires: Sep  4 05:59:35 2026 GMT
  host: saharaai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 03:16:48 2027 GMT
  host: app.saharaai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: portal.saharalabs.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''portal.saha'
kind: domain-security
layout: security
method: probed
name: Sahara Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sahara AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sahara AI
provider_slug: sahara-ai
slug: sahara-ai-domain-security
source_filename: sahara-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saharaai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 05:59:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.saharaai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 03:16:48 2027 GMT\n  hsts: false\n- host: portal.saharalabs.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''portal.saha'\n  hsts: null\ndomains:\n- domain: saharaai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: saharalabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sahara-ai/refs/heads/main/security/sahara-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Artificial Intelligence
- Machine Learning
- Agents
- Compute
- Blockchain
- Inference
- Data
---
