---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bloomnation.com
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.bloomnation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomnation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BloomNation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BloomNation
provider_slug: bloomnation
slug: bloomnation-domain-security
source_filename: bloomnation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomnation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bloomnation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomnation/refs/heads/main/security/bloomnation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Flowers
- Floral Delivery
- Marketplace
- E-Commerce
- Local Florists
- Same-Day Delivery
- Retail
- Payments
- Consumer
---
