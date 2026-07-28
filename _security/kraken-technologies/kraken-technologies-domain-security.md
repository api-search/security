---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kraken.tech
  spf: true
hosts:
- cert_expires: Sep 19 20:15:03 2026 GMT
  host: www.kraken.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: docs.kraken.tech
  hsts: false
  https: true
  note: Documentation portal (Django). Manually probed 2026-07-27 — not covered by the automated pass because it is not an apis.yml baseURL. Negotiates TLS 1.2 (no TLS 1.3) and sends no Strict-Transport-Security header, which is weaker than the marketing host.
  server: gunicorn
  tls_version: TLSv1.2
  x_frame_options: DENY
- cert_expires: Oct 11 14:37:21 2026 GMT
  host: tako.kraken.tech
  hsts: false
  https: true
  note: Tako design-system docs, served by GitHub Pages (CNAME to octoenergy.github.io). Manually probed 2026-07-27. No HSTS header.
  server: GitHub.com
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kraken Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kraken Technologies, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kraken Technologies
provider_slug: kraken-technologies
slug: kraken-technologies-domain-security
source_filename: kraken-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts, plus manual host probes of docs.kraken.tech and tako.kraken.tech (2026-07-27)\nhosts:\n- host: www.kraken.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:15:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.kraken.tech\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\n  server: gunicorn\n  x_frame_options: DENY\n  note: >-\n    Documentation portal (Django). Manually probed 2026-07-27 — not covered by the automated pass\n    because it is not an apis.yml baseURL. Negotiates TLS 1.2 (no TLS 1.3) and sends no\n    Strict-Transport-Security header, which is weaker than the marketing host.\n- host: tako.kraken.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:37:21 2026 GMT\n  hsts: false\n  server: GitHub.com\n  note: >-\n    Tako design-system docs, served by GitHub Pages\
  \ (CNAME to octoenergy.github.io). Manually probed\n    2026-07-27. No HSTS header.\ndomains:\n- domain: kraken.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kraken-technologies/refs/heads/main/security/kraken-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Demand Response
- DER
- Billing
- Energy Platform
---
