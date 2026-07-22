---
api_specs:
- filename: rill-data-admin-openapi.yaml
  format: yaml
  label: Rill Admin API
  slug: rill-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rill-data/refs/heads/main/openapi/rill-data-admin-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: rilldata.com
  spf: true
hosts:
- cert_expires: Sep 24 08:04:09 2026 GMT
  host: www.rilldata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rill Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rill Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Rill Data
provider_slug: rill-data
slug: rill-data-domain-security
source_filename: rill-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rilldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:04:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rilldata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rill-data/refs/heads/main/security/rill-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Analytics
- Business Intelligence
- Dashboards
- Metrics
- Data
- OLAP
- Open Source
- Developer Tools
---
