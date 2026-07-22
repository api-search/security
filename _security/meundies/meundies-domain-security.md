---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meundies.com
  spf: true
hosts:
- cert_expires: Oct  8 20:50:09 2026 GMT
  host: meundies.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meundies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MeUndies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MeUndies
provider_slug: meundies
slug: meundies-domain-security
source_filename: meundies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meundies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 20:50:09 2026 GMT\n  hsts: null\ndomains:\n- domain: meundies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meundies/refs/heads/main/security/meundies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Retail
- Apparel
- Direct-to-Consumer
- Subscription
- Consumer Products
---
