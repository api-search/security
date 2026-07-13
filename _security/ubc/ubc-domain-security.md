---
api_specs:
- filename: ubc-abacus-dataverse.yaml
  format: yaml
  label: UBC Abacus Dataverse API
  slug: abacus-dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubc/refs/heads/main/openapi/ubc-abacus-dataverse.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ubc.ca
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: www.ubc.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 19:27:06 2026 GMT
  host: open.library.ubc.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: oc-index.library.ubc.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of British Columbia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of British Columbia
provider_slug: ubc
slug: ubc-domain-security
source_filename: ubc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ubc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open.library.ubc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 19:27:06 2026 GMT\n  hsts: false\n- host: oc-index.library.ubc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ubc.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubc/refs/heads/main/security/ubc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Canada
- Library
- Open Data
- Research Data
- Digital Collections
---
