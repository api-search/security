---
api_specs:
- filename: uppsala-ucdp.yaml
  format: yaml
  label: UCDP API
  slug: ucdp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-ucdp.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uu.se
  spf: true
hosts:
- cert_expires: Sep 20 02:18:39 2026 GMT
  host: www.uu.se
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 10:50:19 2026 GMT
  host: ucdp.uu.se
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 10:45:11 2026 GMT
  host: ucdpapi.pcr.uu.se
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uppsala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uppsala University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Uppsala University
provider_slug: uppsala
slug: uppsala-domain-security
source_filename: uppsala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uu.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:18:39 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: ucdp.uu.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:50:19 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: ucdpapi.pcr.uu.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:45:11 2026 GMT\n  hsts: null\ndomains:\n- domain: uu.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/security/uppsala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Sweden
---
