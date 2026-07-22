---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: salasa.co
  spf: true
hosts:
- cert_expires: Oct  9 01:03:27 2026 GMT
  host: salasa.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salasa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salasa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Salasa
provider_slug: salasa
slug: salasa-domain-security
source_filename: salasa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: salasa.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:03:27 2026 GMT\n  hsts: false\ndomains:\n- domain: salasa.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salasa/refs/heads/main/security/salasa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Fulfillment
- eCommerce
- Shipping
- Supply Chain
- Saudi Arabia
- Warehousing
---
