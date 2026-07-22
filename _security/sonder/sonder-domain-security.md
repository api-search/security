---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sonder.com
  spf: true
hosts:
- cert_expires: Oct  2 05:43:11 2026 GMT
  host: www.sonder.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sonder
provider_slug: sonder
slug: sonder-domain-security
source_filename: sonder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sonder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:43:11 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: sonder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonder/refs/heads/main/security/sonder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Hospitality
- Travel
- Lodging
- Short-Term Rental
- Accommodations
---
