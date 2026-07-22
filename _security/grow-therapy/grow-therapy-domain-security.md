---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: growtherapy.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: growtherapy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grow Therapy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grow Therapy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Grow Therapy
provider_slug: grow-therapy
slug: grow-therapy-domain-security
source_filename: grow-therapy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: growtherapy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: growtherapy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grow-therapy/refs/heads/main/security/grow-therapy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mental Health
- Telehealth
- Healthcare
- Therapy
- Medication Management
- Insurance
- Marketplace
- Behavioral Health
---
