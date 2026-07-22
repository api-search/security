---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: purmeo.de
  spf: false
hosts:
- cert_expires: Aug 20 09:42:34 2026 GMT
  host: purmeo.de
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Purmeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Purmeo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Purmeo
provider_slug: purmeo
slug: purmeo-domain-security
source_filename: purmeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: purmeo.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 09:42:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: purmeo.de\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purmeo/refs/heads/main/security/purmeo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Nutritional Supplements
- Health and Wellness
- Vitamins
- Ecommerce
- Consumer Health
- Germany
---
