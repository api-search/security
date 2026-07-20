---
api_specs:
- filename: edge-delta-openapi-original.json
  format: json
  label: Edge Delta API
  slug: edge-delta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/openapi/edge-delta-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: edgedelta.com
  spf: true
hosts:
- cert_expires: Sep 13 01:22:57 2026 GMT
  host: edgedelta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.edgedelta.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edge Delta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edge Delta, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Edge Delta
provider_slug: edge-delta
slug: edge-delta-domain-security
source_filename: edge-delta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edgedelta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 01:22:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.edgedelta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: edgedelta.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edge-delta/refs/heads/main/security/edge-delta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Observability
- Telemetry Pipelines
- Logging
- Metrics
- Tracing
- Monitoring
- DevOps
- SRE
- AI
---
