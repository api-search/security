---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: climacell.co
  spf: true
  spf_note: includes tomorrow.io — confirms same organization
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tomorrow.io
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M01
  host: climacell.co
  hsts: null
  https: true
  note: 301-redirects to https://www.tomorrow.io (legacy ClimaCell domain)
  tls_version: TLSv1.3
- cert_expires: Sep 25 09:54:35 2026 GMT
  host: www.tomorrow.io
  hsts: null
  https: true
  note: successor Tomorrow.io host
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Climacell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Climacell, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Climacell
provider_slug: climacell
slug: climacell-domain-security
source_filename: climacell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: climacell.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  cert_issuer: Amazon RSA 2048 M01\n  hsts: null\n  note: 301-redirects to https://www.tomorrow.io (legacy ClimaCell domain)\n- host: www.tomorrow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 09:54:35 2026 GMT\n  hsts: null\n  note: successor Tomorrow.io host\ndomains:\n- domain: climacell.co\n  dnssec: false\n  caa: []\n  spf: true\n  spf_note: 'includes tomorrow.io — confirms same organization'\n  dmarc: true\n  dmarc_policy: reject\n- domain: tomorrow.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climacell/refs/heads/main/security/climacell-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Forecast
- Climate
- Weather Intelligence
- Air Quality
- Precipitation
- Weather of Things
- Geospatial
- Risk
- Alerts
---
