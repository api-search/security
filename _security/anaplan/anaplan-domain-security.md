---
api_specs:
- filename: anaplaninc
  format: yaml
  label: Anaplan Integration API v2.0
  slug: anaplan-integration-api-v20
  spec_type: Postman
  url: https://www.postman.com/anaplaninc
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anaplan.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: www.anaplan.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: help.anaplan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api.anaplan.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anaplan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anaplan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anaplan
provider_slug: anaplan
slug: anaplan-domain-security
source_filename: anaplan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anaplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.anaplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\n- host: api.anaplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: anaplan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anaplan/refs/heads/main/security/anaplan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connected Planning
- Enterprise Planning
- FP&A
- Supply Chain
- Sales Planning
- Financial Consolidation
- SCIM
- REST
---
