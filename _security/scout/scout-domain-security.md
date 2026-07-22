---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: scout.space
  spf: true
hosts:
- cert_expires: Aug 24 04:15:39 2026 GMT
  host: scout.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Scout
provider_slug: scout
slug: scout-domain-security
source_filename: scout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scout.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 04:15:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scout.space\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scout/refs/heads/main/security/scout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Space
- Aerospace
- Satellite
- Space Domain Awareness
- Defense
- Sensors
- Autonomy
---
