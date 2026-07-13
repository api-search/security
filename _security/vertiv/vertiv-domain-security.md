---
api_specs:
- filename: vertiv-environet-alert-openapi.yml
  format: yaml
  label: Vertiv Environet Alert REST API
  slug: environet-alert-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/openapi/vertiv-environet-alert-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vertiv.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: geistglobal.com
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.vertiv.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 20:11:54 2026 GMT
  host: www.geistglobal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vertiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vertiv, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vertiv
provider_slug: vertiv
slug: vertiv-domain-security
source_filename: vertiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vertiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.geistglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:11:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vertiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: geistglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertiv/refs/heads/main/security/vertiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Critical Infrastructure
- Data Center
- DCIM
- Infrastructure Monitoring
- Power Management
- UPS
---
