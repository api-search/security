---
api_specs:
- filename: dnv-class-status-openapi.yml
  format: yaml
  label: DNV Class Status API
  slug: dnv-class-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnv/refs/heads/main/openapi/dnv-class-status-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dnv.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: veracity.com
  spf: true
hosts:
- cert_expires: Oct  8 06:15:51 2026 GMT
  host: www.dnv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 10:19:15 2026 GMT
  host: www.veracity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: maritime.dnv.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dnv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNV, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DNV
provider_slug: dnv
slug: dnv-domain-security
source_filename: dnv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dnv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 06:15:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.veracity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 10:19:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: maritime.dnv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dnv.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: veracity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnv/refs/heads/main/security/dnv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Maritime
- Energy
- Classification
- Vessel
- Data Platform
---
