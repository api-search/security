---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: breathewellbeing.in
  spf: true
hosts:
- cert_expires: Jan  1 13:10:37 2027 GMT
  host: www.breathewellbeing.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Breathe Well Being Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breathe Well-being, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Breathe Well-being
provider_slug: breathe-well-being
slug: breathe-well-being-domain-security
source_filename: breathe-well-being-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breathewellbeing.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 13:10:37 2027 GMT\n  hsts: false\ndomains:\n- domain: breathewellbeing.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breathe-well-being/refs/heads/main/security/breathe-well-being-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Digital Therapeutics
- Diabetes
- Chronic Care
- Wellness
- Mobile App
- India
---
