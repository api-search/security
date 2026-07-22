---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: viralgains.com
  spf: true
hosts:
- cert_expires: Sep  6 15:32:09 2026 GMT
  host: viralgains.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Viralgains Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ViralGains, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ViralGains
provider_slug: viralgains
slug: viralgains-domain-security
source_filename: viralgains-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: viralgains.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:32:09 2026 GMT\n  hsts: false\ndomains:\n- domain: viralgains.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viralgains/refs/heads/main/security/viralgains-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- AdTech
- Zero-Party Data
- Marketing
- Brand Lift
- Consumer Insights
- Health and Pharma
---
