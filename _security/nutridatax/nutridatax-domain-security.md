---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nutridatax.com
  spf: true
hosts:
- cert_expires: Dec 26 21:11:43 2026 GMT
  host: nutridatax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nutridatax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NutriDataX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NutriDataX
provider_slug: nutridatax
slug: nutridatax-domain-security
source_filename: nutridatax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nutridatax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 21:11:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nutridatax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutridatax/refs/heads/main/security/nutridatax-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Nutrition
- FoodData
- API
- AI
---
