---
api_specs:
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Web Endpoints API
  slug: beam-cloud-web-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Task Queues API
  slug: beam-cloud-task-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Tasks Management API
  slug: beam-cloud-tasks-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
- filename: beam-cloud-openapi.yml
  format: yaml
  label: Beam Sandboxes and Volumes API
  slug: beam-cloud-sandboxes-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/openapi/beam-cloud-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beam.cloud
  spf: true
hosts:
- cert_expires: Aug 29 11:09:17 2026 GMT
  host: www.beam.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 07:25:40 2026 GMT
  host: docs.beam.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: app.beam.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beam Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beam
provider_slug: beam-cloud
slug: beam-cloud-domain-security
source_filename: beam-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beam.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 11:09:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.beam.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:25:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.beam.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: beam.cloud\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beam-cloud/refs/heads/main/security/beam-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Serverless
- GPU
- Python
- Inference
- Containers
---
