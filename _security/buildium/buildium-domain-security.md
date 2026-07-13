---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buildium.com
  spf: true
hosts:
- cert_expires: Aug 27 02:43:28 2026 GMT
  host: www.buildium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: api.buildium.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buildium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buildium, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Buildium
provider_slug: buildium
slug: buildium-domain-security
source_filename: buildium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buildium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:43:28 2026 GMT\n  hsts: false\n- host: api.buildium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: buildium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildium/refs/heads/main/security/buildium-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Property Management
- Residential
- Community Associations
- Accounting
- PropTech
- SMB
---
