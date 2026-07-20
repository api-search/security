---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 99minutos.com
  spf: true
hosts:
- cert_expires: Oct 12 16:00:02 2026 GMT
  host: 99minutos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 99Minutos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 99minutos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 99minutos
provider_slug: 99minutos
slug: 99minutos-domain-security
source_filename: 99minutos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 99minutos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 16:00:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 99minutos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/99minutos/refs/heads/main/security/99minutos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Shipping
- Last-Mile Delivery
- Ecommerce
- Fulfillment
- Package Tracking
- Latin America
- Parcel Delivery
- Webhooks
---
