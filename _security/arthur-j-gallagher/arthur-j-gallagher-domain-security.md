---
api_specs:
- filename: gallagher-command-centre-api.yml
  format: yaml
  label: Gallagher Command Centre REST API
  slug: command-centre-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-j-gallagher/refs/heads/main/openapi/gallagher-command-centre-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ajg.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gallagherbassett.com
  spf: true
hosts:
- cert_expires: Aug 11 23:59:59 2026 GMT
  host: www.ajg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: developer.gallagherbassett.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.gallagherbassett.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arthur J Gallagher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arthur J. Gallagher, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arthur J. Gallagher
provider_slug: arthur-j-gallagher
slug: arthur-j-gallagher-domain-security
source_filename: arthur-j-gallagher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ajg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.gallagherbassett.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gallagherbassett.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ajg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gallagherbassett.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arthur-j-gallagher/refs/heads/main/security/arthur-j-gallagher-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Brokerage
- Risk Management
- Claims Management
- Security
- Benefits
- Fortune 1000
---
