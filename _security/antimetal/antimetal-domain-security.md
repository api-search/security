---
api_specs:
- filename: antimetal-artifacts-api-openapi.yml
  format: yaml
  label: Antimetal Artifacts API
  slug: antimetal-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-artifacts-api-openapi.yml
- filename: antimetal-issues-api-openapi.yml
  format: yaml
  label: Antimetal Issues API
  slug: antimetal-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-issues-api-openapi.yml
- filename: antimetal-query-api-openapi.yml
  format: yaml
  label: Antimetal Query API
  slug: antimetal-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/openapi/antimetal-query-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: antimetal.com
  spf: true
hosts:
- cert_expires: Sep 22 13:42:03 2026 GMT
  host: www.antimetal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 12:07:54 2026 GMT
  host: docs.antimetal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 09:18:21 2026 GMT
  host: bff.antimetal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Antimetal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antimetal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Antimetal
provider_slug: antimetal
slug: antimetal-domain-security
source_filename: antimetal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.antimetal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:42:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.antimetal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 12:07:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: bff.antimetal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 09:18:21 2026 GMT\n  hsts: null\ndomains:\n- domain: antimetal.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antimetal/refs/heads/main/security/antimetal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Observability
- Incident Management
- Site Reliability Engineering
- Artificial Intelligence
- Agents
- DevOps
- Cloud Infrastructure
- Kubernetes
- Root Cause Analysis
- MCP
---
