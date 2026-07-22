---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snaproute.com
  spf: true
hosts:
- cert_expires: Oct 12 05:27:35 2026 GMT
  host: snaproute.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snaproute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snaproute, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Snaproute
provider_slug: snaproute
slug: snaproute-domain-security
source_filename: snaproute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snaproute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:27:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: snaproute.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snaproute/refs/heads/main/security/snaproute-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Networking
- Network Operating System
- Cloud Native
- SDN
- Infrastructure
- Defunct
---
