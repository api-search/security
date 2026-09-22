---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paris.fr
  spf: true
hosts:
- cert_expires: Dec 17 20:48:12 2026 GMT
  host: opendata.paris.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opendata Paris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paris Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Paris Open Data
provider_slug: opendata-paris
slug: opendata-paris-domain-security
source_filename: opendata-paris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.paris.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 20:48:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paris.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-paris/refs/heads/main/security/opendata-paris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- OpenData
- Government
- Transparency
- Paris
---
