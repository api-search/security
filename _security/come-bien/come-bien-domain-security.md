---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: comebien.mx
  spf: true
hosts:
- cert_expires: Sep 23 22:03:32 2026 GMT
  host: comebien.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Come Bien Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Come Bien, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Come Bien
provider_slug: come-bien
slug: come-bien-domain-security
source_filename: come-bien-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: comebien.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:03:32 2026 GMT\n  hsts: false\ndomains:\n- domain: comebien.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/come-bien/refs/heads/main/security/come-bien-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food
- FoodTech
- Meal Delivery
- Corporate Catering
- Employee Benefits
- Mexico
- Subscription
---
