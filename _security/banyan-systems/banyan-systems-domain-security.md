---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: banyan.com
  spf: true
hosts:
- cert_expires: Aug 23 06:26:40 2026 GMT
  host: developers.banyan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 08:57:49 2026 GMT
  host: api.banyan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Banyan Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banyan Systems, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Banyan Systems
provider_slug: banyan-systems
slug: banyan-systems-domain-security
source_filename: banyan-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.banyan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:26:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.banyan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:57:49 2026 GMT\n  hsts: false\ndomains:\n- domain: banyan.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/security/banyan-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Receipt Data
- Transaction Enrichment
- Item-Level Data
- Card-Linked Offers
- Fintech
- Payments
- Data Collaboration
- Webhooks
---
