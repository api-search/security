---
api_specs:
- filename: mithril-compute-openapi-original.json
  format: json
  label: Mithril Compute API
  slug: mithril-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-compute-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mithril.ai
  spf: true
hosts:
- cert_expires: Aug 24 10:31:28 2026 GMT
  host: mithril.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  6 21:04:00 2026 GMT
  host: api.mithril.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mithril Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mithril, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mithril
provider_slug: mithril
slug: mithril-domain-security
source_filename: mithril-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mithril.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:31:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mithril.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 21:04:00 2026 GMT\n  hsts: null\ndomains:\n- domain: mithril.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/security/mithril-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- GPU Cloud
- AI Infrastructure
- Machine Learning
- Cloud Computing
- Compute
- Spot Instances
- Kubernetes
- GPU
---
