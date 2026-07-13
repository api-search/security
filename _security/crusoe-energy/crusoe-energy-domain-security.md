---
api_specs:
- filename: crusoe-energy-openapi.json
  format: json
  label: Crusoe Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crusoe-energy/refs/heads/main/openapi/crusoe-energy-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crusoe.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crusoecloud.com
  spf: true
hosts:
- cert_expires: Aug 26 03:28:21 2026 GMT
  host: crusoe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 00:34:15 2026 GMT
  host: docs.crusoecloud.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 00:34:15 2026 GMT
  host: api.crusoecloud.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crusoe Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crusoe, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crusoe
provider_slug: crusoe-energy
slug: crusoe-energy-domain-security
source_filename: crusoe-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crusoe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 03:28:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.crusoecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:34:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.crusoecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:34:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: crusoe.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: crusoecloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crusoe-energy/refs/heads/main/security/crusoe-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Cloud
- GPU
- Compute
- Inference
- Energy
- Sustainability
- NVIDIA
- AMD
- Kubernetes
- Storage
- Networking
- Foundation Models
---
