---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: adviceslip.com
  spf: false
hosts:
- cert_expires: Sep 29 11:03:27 2026 GMT
  host: api.adviceslip.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Advice Slip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advice Slip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Advice Slip
provider_slug: advice-slip
slug: advice-slip-domain-security
source_filename: advice-slip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.adviceslip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:03:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adviceslip.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advice-slip/refs/heads/main/security/advice-slip-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Personality
- Public APIs
---
