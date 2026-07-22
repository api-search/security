---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mosaic.us
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: mosaic.us
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mosaic Building Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mosaic Building Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mosaic Building Group
provider_slug: mosaic-building-group
slug: mosaic-building-group-domain-security
source_filename: mosaic-building-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mosaic.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mosaic.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosaic-building-group/refs/heads/main/security/mosaic-building-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Construction Technology
- Build-to-Rent
- PropTech
- Real Estate
- Homebuilding
- Construction Management
---
