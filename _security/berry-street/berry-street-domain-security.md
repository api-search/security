---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: berrystreet.co
  spf: true
hosts:
- cert_expires: Sep 30 00:54:12 2026 GMT
  host: www.berrystreet.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Berry Street Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Berry Street, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Berry Street
provider_slug: berry-street
slug: berry-street-domain-security
source_filename: berry-street-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.berrystreet.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:54:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: berrystreet.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/berry-street/refs/heads/main/security/berry-street-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Nutrition
- Telehealth
- Dietitian
- Medical Nutrition Therapy
- Insurance
- Digital Health
---
