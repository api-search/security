---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryhampr.com
  spf: true
hosts:
- cert_expires: Oct  7 19:30:47 2026 GMT
  host: tryhampr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hampr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hampr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: hampr
provider_slug: hampr
slug: hampr-domain-security
source_filename: hampr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryhampr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:30:47 2026 GMT\n  hsts: false\ndomains:\n- domain: tryhampr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hampr/refs/heads/main/security/hampr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Laundry
- On-Demand
- Delivery
- Consumer Services
- Mobile App
- Gig Economy
- Commercial Laundry
---
