---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blueplanet.com
  spf: true
hosts:
- cert_expires: Nov  2 19:26:22 2026 GMT
  host: blueplanet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blue Planet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue Planet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blue Planet
provider_slug: blue-planet
slug: blue-planet-domain-security
source_filename: blue-planet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blueplanet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 19:26:22 2026 GMT\n  hsts: null\ndomains:\n- domain: blueplanet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-planet/refs/heads/main/security/blue-planet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- Technology
- Data
- Cloud
---
