---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cowboyspace.com
  spf: true
hosts:
- cert_expires: Oct  7 03:04:19 2026 GMT
  host: cowboyspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cowboy Space Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cowboy Space Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cowboy Space Corporation
provider_slug: cowboy-space-corporation
slug: cowboy-space-corporation-domain-security
source_filename: cowboy-space-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cowboyspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:04:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cowboyspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cowboy-space-corporation/refs/heads/main/security/cowboy-space-corporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Space
- Satellites
- Data Centers
- Artificial Intelligence
- Cloud Computing
- Infrastructure
- Low Earth Orbit
---
