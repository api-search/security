---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: exodigo.com
  spf: true
hosts:
- cert_expires: Oct  6 09:58:30 2026 GMT
  host: www.exodigo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exodigo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exodigo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Exodigo
provider_slug: exodigo
slug: exodigo-domain-security
source_filename: exodigo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exodigo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:58:30 2026 GMT\n  hsts: null\ndomains:\n- domain: exodigo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exodigo/refs/heads/main/security/exodigo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Subsurface Intelligence
- Underground Mapping
- Geophysics
- Infrastructure
- Construction
- Utilities
- Geospatial
- Artificial Intelligence
- Engineering Services
---
