---
api_specs:
- filename: evidence-dev-openapi.yml
  format: yaml
  label: Evidence Framework (SQL + Markdown)
  slug: evidence-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evidence-dev/refs/heads/main/openapi/evidence-dev-openapi.yml
- filename: evidence-dev-openapi.yml
  format: yaml
  label: Evidence USQL / Query Layer
  slug: usql-query-layer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evidence-dev/refs/heads/main/openapi/evidence-dev-openapi.yml
- filename: evidence-dev-openapi.yml
  format: yaml
  label: Evidence Cloud
  slug: evidence-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evidence-dev/refs/heads/main/openapi/evidence-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: evidence.dev
  spf: true
hosts:
- cert_expires: Sep 16 10:59:47 2026 GMT
  host: evidence.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 08:28:20 2026 GMT
  host: docs.evidence.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evidence Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evidence, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Evidence
provider_slug: evidence-dev
slug: evidence-dev-domain-security
source_filename: evidence-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evidence.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:59:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.evidence.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:28:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: evidence.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evidence-dev/refs/heads/main/security/evidence-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Business Intelligence
- BI as Code
- SQL
- Markdown
- Data Apps
- Open Source
---
