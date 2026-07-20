---
api_specs:
- filename: boltz-compute.yml
  format: yaml
  label: Boltz Compute API
  slug: boltz-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boltz/refs/heads/main/openapi/boltz-compute.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boltz.bio
  spf: true
hosts:
- cert_expires: Oct 13 10:49:30 2026 GMT
  host: boltz.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boltz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boltz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boltz
provider_slug: boltz
slug: boltz-domain-security
source_filename: boltz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boltz.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 10:49:30 2026 GMT\n  hsts: false\ndomains:\n- domain: boltz.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltz/refs/heads/main/security/boltz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Digital Biology
- Drug Discovery
- Artificial Intelligence
- Machine Learning
- Protein Design
- Structure Prediction
- Life Sciences
- Compute
---
