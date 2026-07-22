---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: homage.sg
  spf: true
hosts:
- cert_expires: Oct 13 19:46:56 2026 GMT
  host: homage.sg
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Homage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Homage
provider_slug: homage
slug: homage-domain-security
source_filename: homage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homage.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 19:46:56 2026 GMT\n  hsts: false\ndomains:\n- domain: homage.sg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homage/refs/heads/main/security/homage-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Caregiving
- Home Care
- Health Services
- Aged Care
- Telehealth
- Singapore
---
