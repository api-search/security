---
api_specs:
- filename: north-cloud-openapi.yml
  format: yaml
  label: North.Cloud Public API
  slug: north-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/north-cloud/refs/heads/main/openapi/north-cloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: north.cloud
  spf: true
hosts:
- cert_expires: Aug 26 23:17:33 2026 GMT
  host: www.north.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.north.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: North Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for North.Cloud, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: North.Cloud
provider_slug: north-cloud
slug: north-cloud-domain-security
source_filename: north-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.north.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:17:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.north.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: north.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/north-cloud/refs/heads/main/security/north-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinOps
- Cloud Cost Management
- GCP
- Cost Optimization
- Cost Units
---
