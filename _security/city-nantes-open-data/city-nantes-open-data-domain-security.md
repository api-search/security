---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nantesmetropole.fr
  spf: true
hosts:
- cert_expires: Aug 19 10:13:59 2026 GMT
  host: data.nantesmetropole.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: City Nantes Open Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City, Nantes Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: City, Nantes Open Data
provider_slug: city-nantes-open-data
slug: city-nantes-open-data-domain-security
source_filename: city-nantes-open-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.nantesmetropole.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 10:13:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nantesmetropole.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/city-nantes-open-data/refs/heads/main/security/city-nantes-open-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Public APIs
---
