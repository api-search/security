---
description: ''
domains:
- caa:
  - 0 iodef "mailto:domains@mercadolibre.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mercadolibre.cl
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: developers.mercadolibre.cl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercadolibre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercadolibre, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mercadolibre
provider_slug: mercadolibre
slug: mercadolibre-domain-security
source_filename: mercadolibre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.mercadolibre.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mercadolibre.cl\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:domains@mercadolibre.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercadolibre/refs/heads/main/security/mercadolibre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shopping
- Public APIs
---
