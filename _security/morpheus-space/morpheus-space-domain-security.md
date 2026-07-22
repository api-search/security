---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: morpheus.space
  spf: true
hosts:
- cert_expires: Oct  9 23:42:06 2026 GMT
  host: morpheus.space
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morpheus Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morpheus Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Morpheus Space
provider_slug: morpheus-space
slug: morpheus-space-domain-security
source_filename: morpheus-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: morpheus.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:42:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: morpheus.space\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morpheus-space/refs/heads/main/security/morpheus-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Space
- Satellite
- Propulsion
- Electric Propulsion
- Aerospace
- Mission Design
- New Space
---
