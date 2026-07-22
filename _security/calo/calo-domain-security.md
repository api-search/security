---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: calo.app
  spf: true
hosts:
- cert_expires: Sep 23 07:17:33 2026 GMT
  host: calo.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Calo
provider_slug: calo
slug: calo-domain-security
source_filename: calo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:17:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: calo.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calo/refs/heads/main/security/calo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food
- Meal Delivery
- Meal Plans
- Nutrition
- Health
- Subscription
- Food Tech
---
