---
api_specs:
- filename: state-farm-insurance-cos-renters-openapi.yml
  format: yaml
  label: Renters Insurance API
  slug: renters-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/state-farm-insurance-cos/refs/heads/main/openapi/state-farm-insurance-cos-renters-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "microsoft.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: statefarm.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.statefarm.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: developer.statefarm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.statefarm.com
  https: false
kind: domain-security
layout: security
method: probed
name: State Farm Insurance Cos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for State Farm Insurance Companies, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: State Farm Insurance Companies
provider_slug: state-farm-insurance-cos
slug: state-farm-insurance-cos-domain-security
source_filename: state-farm-insurance-cos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.statefarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer.statefarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\n- host: api.statefarm.com\n  https: false\ndomains:\n- domain: statefarm.com\n  dnssec: false\n  caa:\n  - 0 issue \"microsoft.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-farm-insurance-cos/refs/heads/main/security/state-farm-insurance-cos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
