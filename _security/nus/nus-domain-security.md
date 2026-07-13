---
api_specs:
- filename: nus-nusmods.yaml
  format: yaml
  label: NUSMods API (Unofficial / Community)
  slug: nusmods
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/openapi/nus-nusmods.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nus.edu.sg
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nusmods.com
  spf: true
hosts:
- cert_expires: Sep 29 02:20:51 2026 GMT
  host: nus.edu.sg
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 06:49:35 2026 GMT
  host: scholarbank.nus.edu.sg
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 03:57:51 2026 GMT
  host: api.nusmods.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National University of Singapore, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: National University of Singapore
provider_slug: nus
slug: nus-domain-security
source_filename: nus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nus.edu.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:20:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: scholarbank.nus.edu.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 06:49:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.nusmods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:57:51 2026 GMT\n  hsts: false\ndomains:\n- domain: nus.edu.sg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nusmods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/security/nus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Singapore
- Research
- Open Access
- Repository
---
