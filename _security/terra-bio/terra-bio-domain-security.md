---
api_specs:
- filename: terra-bio-public-api-openapi.yml
  format: yaml
  label: Terra Public API
  slug: terra-bio-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-bio/refs/heads/main/openapi/terra-bio-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: terra.bio
  spf: true
hosts:
- cert_expires: Nov 28 10:57:47 2026 GMT
  host: terra.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Terra Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Terra
provider_slug: terra-bio
slug: terra-bio-domain-security
source_filename: terra-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terra.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:57:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: terra.bio\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terra-bio/refs/heads/main/security/terra-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Biomedical
- DataAnalysis
- Collaboration
- CloudPlatform
---
