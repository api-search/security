---
api_specs:
- filename: dott-gbfs-openapi.yml
  format: yaml
  label: Dott GBFS API
  slug: dott-gbfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dott/refs/heads/main/openapi/dott-gbfs-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ridedott.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: ridedott.dev
  spf: true
hosts:
- cert_expires: Sep  8 07:04:44 2026 GMT
  host: ridedott.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 05:24:23 2026 GMT
  host: ridedott.dev
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 05:24:23 2026 GMT
  host: gbfs.api.ridedott.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dott Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dott, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dott
provider_slug: dott
slug: dott-domain-security
source_filename: dott-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ridedott.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 07:04:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ridedott.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 05:24:23 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: gbfs.api.ridedott.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 05:24:23 2026 GMT\n  hsts: null\ndomains:\n- domain: ridedott.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ridedott.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dott/refs/heads/main/security/dott-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Transportation
- Micromobility
- Mobility
- E-Scooter
- E-Bike
- GBFS
- Shared Mobility
- Smart City
- Sustainability
---
