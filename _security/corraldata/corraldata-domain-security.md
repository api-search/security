---
api_specs:
- filename: corraldata-kb-api-openapi.yml
  format: yaml
  label: CorralData Kb API
  slug: corraldata-kb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corraldata/refs/heads/main/openapi/corraldata-kb-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: corraldata.com
  spf: true
hosts:
- cert_expires: Dec 13 22:23:49 2026 GMT
  host: corraldata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corraldata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CorralData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CorralData
provider_slug: corraldata
slug: corraldata-domain-security
source_filename: corraldata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corraldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 22:23:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corraldata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corraldata/refs/heads/main/security/corraldata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Analytics
- Healthcare
- Artificial Intelligence
- Platform
---
