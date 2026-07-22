---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: voygr.tech
  spf: true
hosts:
- cert_expires: Aug 25 08:15:11 2026 GMT
  host: voygr.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voygr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VOYGR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VOYGR
provider_slug: voygr
slug: voygr-domain-security
source_filename: voygr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voygr.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 08:15:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: voygr.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voygr/refs/heads/main/security/voygr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Location Intelligence
- POI Data
- Data Enrichment
- Data Validation
- Geospatial
- Places
- AI Agents
- Y Combinator
---
