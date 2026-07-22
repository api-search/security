---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bloomon.co.uk
  spf: true
hosts:
- cert_expires: Sep 27 15:28:59 2026 GMT
  host: www.bloomon.co.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bloomon
provider_slug: bloomon
slug: bloomon-domain-security
source_filename: bloomon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomon.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:28:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: bloomon.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomon/refs/heads/main/security/bloomon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Flowers
- Flower Delivery
- Subscription
- E-Commerce
- Gifting
- Retail
- Bloom & Wild Group
---
