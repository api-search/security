---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spocket.co
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: spocket.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spocket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spocket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spocket
provider_slug: spocket
slug: spocket-domain-security
source_filename: spocket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spocket.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: spocket.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spocket/refs/heads/main/security/spocket-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Dropshipping
- E-commerce
- Order Fulfillment
- Product Sourcing
- Suppliers
- Retail
- Marketplace
---
