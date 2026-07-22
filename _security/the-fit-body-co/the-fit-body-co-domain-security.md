---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fitbody.mx
  spf: true
hosts:
- cert_expires: Aug 28 08:08:32 2026 GMT
  host: fitbody.mx
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Fit Body Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Fit Body Co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Fit Body Co
provider_slug: the-fit-body-co
slug: the-fit-body-co-domain-security
source_filename: the-fit-body-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fitbody.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:08:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: fitbody.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-fit-body-co/refs/heads/main/security/the-fit-body-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports Nutrition
- Dietary Supplements
- E-commerce
- Health and Wellness
- Consumer Products
- Mexico
- Shopify
---
