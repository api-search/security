---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: petcircle.com.au
  spf: true
hosts:
- cert_expires: Oct  1 08:48:02 2026 GMT
  host: www.petcircle.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pet Circle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pet Circle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pet Circle
provider_slug: pet-circle
slug: pet-circle-domain-security
source_filename: pet-circle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.petcircle.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:48:02 2026 GMT\n  hsts: null\ndomains:\n- domain: petcircle.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pet-circle/refs/heads/main/security/pet-circle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- E-Commerce
- Pets
- Consumer
- Australia
- Direct To Consumer
- Pet Supplies
- Headless Commerce
---
