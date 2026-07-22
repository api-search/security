---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: siemens-energy.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: www.siemens-energy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dresser Rand Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dresser-Rand Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dresser-Rand Group
provider_slug: dresser-rand-group
slug: dresser-rand-group-domain-security
source_filename: dresser-rand-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.siemens-energy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: siemens-energy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dresser-rand-group/refs/heads/main/security/dresser-rand-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial
- Oil and Gas
- Rotating Equipment
- Energy
---
