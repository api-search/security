---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eksab.com
  spf: true
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: eksab.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Eksab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eksab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eksab
provider_slug: eksab
slug: eksab-domain-security
source_filename: eksab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eksab.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: eksab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eksab/refs/heads/main/security/eksab-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fantasy Sports
- Daily Fantasy Sports
- Sports
- Gaming
- Predictions
- Football
- Egypt
- MENA
---
