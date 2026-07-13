---
api_specs:
- filename: soda-data-openapi.yml
  format: yaml
  label: Soda
  slug: soda-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/openapi/soda-data-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soda.io
  spf: false
hosts:
- cert_expires: Oct  3 15:10:10 2026 GMT
  host: www.soda.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: cloud.soda.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: cloud.us.soda.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soda Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soda, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Soda
provider_slug: soda-data
slug: soda-data-domain-security
source_filename: soda-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:10:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.soda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\n- host: cloud.us.soda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: soda.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soda-data/refs/heads/main/security/soda-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- Data Quality
---
