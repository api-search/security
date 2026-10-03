---
api_specs:
- filename: branch-metrics-openapi-generated.yml
  format: yaml
  label: Branch Metrics API
  slug: branch-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/branch-metrics/refs/heads/main/openapi/_ae-authored/branch-metrics-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
hosts:
- cert_expires: Dec 18 16:17:45 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Branch Metrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branch Metrics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Branch Metrics
provider_slug: branch-metrics
slug: branch-metrics-domain-security
source_filename: branch-metrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 16:17:45 2026 GMT\n  hsts: null\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branch-metrics/refs/heads/main/security/branch-metrics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Mobile
- Attribution
- Deep-Linking
- Marketing
- Analytics
- AI
---
