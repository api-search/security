---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aeroseal.com
  spf: true
hosts:
- cert_expires: Sep 23 20:13:04 2026 GMT
  host: aeroseal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aeroseal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aeroseal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Aeroseal
provider_slug: aeroseal
slug: aeroseal-domain-security
source_filename: aeroseal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aeroseal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:13:04 2026 GMT\n  hsts: false\ndomains:\n- domain: aeroseal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeroseal/refs/heads/main/security/aeroseal-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Energy Efficiency
- Climate Technology
- HVAC
- Building Envelope
- Duct Sealing
- Indoor Air Quality
- Building Performance
- Construction Technology
---
