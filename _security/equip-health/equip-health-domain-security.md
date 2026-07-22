---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: equip.health
  spf: true
hosts:
- cert_expires: Sep  3 03:17:53 2026 GMT
  host: equip.health
  hsts: true
  hsts_max_age: 345600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Equip Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equip Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Equip Health
provider_slug: equip-health
slug: equip-health-domain-security
source_filename: equip-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: equip.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 03:17:53 2026 GMT\n  hsts: true\n  hsts_max_age: 345600\ndomains:\n- domain: equip.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equip-health/refs/heads/main/security/equip-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Telehealth
- Mental Health
- Eating Disorder Treatment
- Virtual Care
- Health Insurance
---
