---
api_specs:
- filename: prefect-openapi.json
  format: json
  label: Prefect Cloud REST API
  slug: prefect-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prefect/refs/heads/main/openapi/prefect-openapi.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:security-notifications@prefect.io"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: prefect.io
  spf: true
hosts:
- cert_expires: Sep 11 17:12:50 2026 GMT
  host: www.prefect.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 23:51:05 2026 GMT
  host: docs.prefect.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prefect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prefect, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Prefect
provider_slug: prefect
slug: prefect-domain-security
source_filename: prefect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prefect.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 17:12:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.prefect.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:51:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: prefect.io\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security-notifications@prefect.io\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prefect/refs/heads/main/security/prefect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- Data Pipelines
- Orchestration
- Python
- Workflows
---
