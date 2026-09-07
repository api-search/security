---
api_specs:
- filename: consolidated-edison-green-button-connect-openapi.yml
  format: yaml
  label: Green Button Connect My Data
  slug: green-button-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/openapi/consolidated-edison-green-button-connect-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coned.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.coned.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.coned.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Consolidated Edison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Consolidated Edison, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Consolidated Edison
provider_slug: consolidated-edison
slug: consolidated-edison-domain-security
source_filename: consolidated-edison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coned.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coned.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coned.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consolidated-edison/refs/heads/main/security/consolidated-edison-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AMI
- Demand Response
- ESPI
- Energy
- Fortune 500
- Green Button
- Interval Data
- NAESB
- Natural Gas
- New York
- OAuth2
- Steam
- Utility
---
