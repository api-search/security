---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: calvis.com
  spf: true
hosts:
- cert_expires: Aug 29 18:50:44 2026 GMT
  host: calvis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calvis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calvis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Calvis
provider_slug: calvis
slug: calvis-domain-security
source_filename: calvis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calvis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:50:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: calvis.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calvis/refs/heads/main/security/calvis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Physical Security
- Security Guards
- Marketplace
- Public Safety
- Workforce
- On-Demand
- Artificial Intelligence
---
