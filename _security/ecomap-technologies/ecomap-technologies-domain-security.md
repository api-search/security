---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ecomap.tech
  spf: true
hosts:
- cert_expires: Sep  3 19:08:36 2026 GMT
  host: ecomap.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ecomap Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EcoMap Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EcoMap Technologies
provider_slug: ecomap-technologies
slug: ecomap-technologies-domain-security
source_filename: ecomap-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecomap.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:08:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ecomap.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecomap-technologies/refs/heads/main/security/ecomap-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Economic Development
- Ecosystem Intelligence
- Ecosystem Mapping
- Resource Navigation
- Nonprofit
- State and Local Government
- Chambers of Commerce
- Artificial Intelligence
- Analytics
- SaaS
---
