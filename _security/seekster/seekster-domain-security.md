---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seekster.co
  spf: true
hosts:
- cert_expires: Sep  7 06:08:15 2026 GMT
  host: seekster.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seekster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seekster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Seekster
provider_slug: seekster
slug: seekster-domain-security
source_filename: seekster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seekster.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 06:08:15 2026 GMT\n  hsts: null\ndomains:\n- domain: seekster.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seekster/refs/heads/main/security/seekster-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- On-Demand Services
- Home Services
- Field Service Management
- Marketplace
- Facility Management
- Thailand
- Services
---
