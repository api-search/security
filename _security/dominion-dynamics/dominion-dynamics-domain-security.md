---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: dominion-dynamics.com
  spf: false
hosts:
- cert_expires: Aug 31 03:00:38 2026 GMT
  host: www.dominion-dynamics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dominion Dynamics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dominion Dynamics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dominion Dynamics
provider_slug: dominion-dynamics
slug: dominion-dynamics-domain-security
source_filename: dominion-dynamics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dominion-dynamics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:00:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dominion-dynamics.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dominion-dynamics/refs/heads/main/security/dominion-dynamics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Deep Tech
- Defense
- National Security
- Autonomy
- Sensing
- Command and Control
- Arctic
- Government
- Canada
---
