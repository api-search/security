---
api_specs:
- filename: ametek-powervar-isite-pro-openapi.yml
  format: yaml
  label: AMETEK Powervar iSite PRO REST API
  slug: powervar-isite-pro
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ametek/refs/heads/main/openapi/ametek-powervar-isite-pro-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "geotrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ametek.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.ametek.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ametek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMETEK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AMETEK
provider_slug: ametek
slug: ametek-domain-security
source_filename: ametek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ametek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ametek.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ametek/refs/heads/main/security/ametek-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Electronic Instruments
- Test and Measurement
- Aerospace
- Energy
- Industrial
- Medical Instruments
- Precision Motion Control
- Manufacturing
- Fortune 1000
---
