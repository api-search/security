---
api_specs:
- filename: invokely-openapi-generated.yml
  format: yaml
  label: Invokely API
  slug: invokely-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invokely/refs/heads/main/openapi/_ae-authored/invokely-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: invokely.ai
  spf: true
hosts:
- cert_expires: Jan  5 21:51:42 2027 GMT
  host: invokely.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Invokely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Invokely, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Invokely
provider_slug: invokely
slug: invokely-domain-security
source_filename: invokely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: invokely.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 21:51:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: invokely.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invokely/refs/heads/main/security/invokely-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Statistics
- Economic Data
- Public Data
- Data API
---
