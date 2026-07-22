---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: govdash.com
  spf: true
hosts:
- cert_expires: Sep 22 22:50:00 2026 GMT
  host: govdash.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Govdash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Govdash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Govdash
provider_slug: govdash
slug: govdash-domain-security
source_filename: govdash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: govdash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:50:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: govdash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govdash/refs/heads/main/security/govdash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government Contracting
- GovCon
- Artificial Intelligence
- Proposal Management
- Capture Management
- Public Sector
- Enterprise
---
