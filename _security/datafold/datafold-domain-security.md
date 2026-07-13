---
api_specs:
- filename: introduction
  format: yaml
  label: Datafold REST API
  slug: datafold-rest-api
  spec_type: OpenAPI
  url: https://docs.datafold.com/api-reference/introduction
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datafold.com
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: www.datafold.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 17:31:16 2026 GMT
  host: docs.datafold.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: app.datafold.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datafold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datafold, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Datafold
provider_slug: datafold
slug: datafold-domain-security
source_filename: datafold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datafold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\n- host: docs.datafold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:31:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.datafold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: datafold.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/security/datafold-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Reliability
- Data Diff
- Data Quality
- Column-Level Lineage
- Data Pipelines
- CI/CD Integration
- Anomaly Detection
- Data Observability
- Data Migrations
---
