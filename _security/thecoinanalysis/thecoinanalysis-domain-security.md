---
api_specs:
- filename: thecoinanalysis-public-api-api-openapi.yml
  format: yaml
  label: The Coin Analysis Public API
  slug: thecoinanalysis-public-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thecoinanalysis/refs/heads/main/openapi/thecoinanalysis-public-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thecoinanalysis.com
  spf: true
hosts:
- cert_expires: Dec 16 20:42:42 2026 GMT
  host: www.thecoinanalysis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thecoinanalysis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Coin Analysis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: The Coin Analysis
provider_slug: thecoinanalysis
slug: thecoinanalysis-domain-security
source_filename: thecoinanalysis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thecoinanalysis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 20:42:42 2026 GMT\n  hsts: false\ndomains:\n- domain: thecoinanalysis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thecoinanalysis/refs/heads/main/security/thecoinanalysis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- News
- Data
---
