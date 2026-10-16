---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: icagruppen.se
  spf: true
hosts:
- cert_expires: Dec 10 11:56:39 2026 GMT
  host: icagruppen.se
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ica Gruppen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ICA Gruppen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ICA Gruppen
provider_slug: ica-gruppen
slug: ica-gruppen-domain-security
source_filename: ica-gruppen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: icagruppen.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 11:56:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: icagruppen.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ica-gruppen/refs/heads/main/security/ica-gruppen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Services
- Sweden
- Sustainability
---
