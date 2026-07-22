---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caresense.ai
  spf: false
hosts:
- cert_expires: Oct 14 12:18:41 2026 GMT
  host: www.caresense.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caresense Pte Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caresense Pte. Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Caresense Pte. Ltd.
provider_slug: caresense-pte-ltd
slug: caresense-pte-ltd-domain-security
source_filename: caresense-pte-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caresense.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 12:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: caresense.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caresense-pte-ltd/refs/heads/main/security/caresense-pte-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Digital Health
- Artificial Intelligence
- Health Coaching
- Preventive Health
- Telemedicine
- Wellness
- Singapore
- Mobile Applications
---
