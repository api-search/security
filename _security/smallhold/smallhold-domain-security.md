---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: smallhold.com
  spf: true
hosts:
- cert_expires: Sep  9 03:24:03 2026 GMT
  host: smallhold.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smallhold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smallhold, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Smallhold
provider_slug: smallhold
slug: smallhold-domain-security
source_filename: smallhold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smallhold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:24:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: smallhold.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smallhold/refs/heads/main/security/smallhold-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Agriculture
- Food and Beverage
- Mushrooms
- Sustainability
- E-commerce
- Consumer Products
---
