---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@hyatt.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hyatt.com
  spf: true
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: www.hyatt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyatt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyatt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hyatt
provider_slug: hyatt
slug: hyatt-domain-security
source_filename: hyatt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyatt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hyatt.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@hyatt.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyatt/refs/heads/main/security/hyatt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hospitality
- Hotels
- Travel
---
