---
api_specs:
- filename: archrock-investor-relations-api.yaml
  format: yaml
  label: Archrock Investor Relations API
  slug: archrock-investor-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/openapi/archrock-investor-relations-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: archrock.com
  spf: true
hosts:
- cert_expires: Sep 30 15:24:13 2026 GMT
  host: www.archrock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.archrock.com
  https: false
kind: domain-security
layout: security
method: probed
name: Archrock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archrock, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Archrock
provider_slug: archrock
slug: archrock-domain-security
source_filename: archrock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.archrock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:24:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.archrock.com\n  https: false\ndomains:\n- domain: archrock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/security/archrock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Natural Gas
- Compression Services
- Oil And Gas
- Energy
- Industrial
- 'NYSE: AROC'
---
