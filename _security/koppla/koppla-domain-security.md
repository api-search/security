---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: koppla.de
  spf: true
hosts:
- cert_expires: Sep 23 09:54:06 2026 GMT
  host: www.koppla.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.koppla.de
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koppla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koppla, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Koppla
provider_slug: koppla
slug: koppla-domain-security
source_filename: koppla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.koppla.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:54:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.koppla.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: koppla.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koppla/refs/heads/main/security/koppla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Construction Technology
- Project Management
- Scheduling
- Lean Construction
- BIM
- Germany
- SaaS
---
