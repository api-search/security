---
api_specs:
- filename: modal-functions-openapi.yml
  format: yaml
  label: Modal Functions API
  slug: modal-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-functions-openapi.yml
- filename: modal-sandboxes-openapi.yml
  format: yaml
  label: Modal Sandboxes API
  slug: modal-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-sandboxes-openapi.yml
- filename: modal-volumes-openapi.yml
  format: yaml
  label: Modal Volumes API
  slug: modal-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-volumes-openapi.yml
- filename: modal-images-openapi.yml
  format: yaml
  label: Modal Images API
  slug: modal-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-images-openapi.yml
- filename: modal-secrets-openapi.yml
  format: yaml
  label: Modal Secrets API
  slug: modal-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-secrets-openapi.yml
- filename: modal-dicts-queues-openapi.yml
  format: yaml
  label: Modal Dicts and Queues API
  slug: modal-dicts-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-dicts-queues-openapi.yml
- filename: modal-schedules-openapi.yml
  format: yaml
  label: Modal Schedules API
  slug: modal-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-schedules-openapi.yml
- filename: modal-web-endpoints-openapi.yml
  format: yaml
  label: Modal Web Endpoints API
  slug: modal-web-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-web-endpoints-openapi.yml
- filename: modal-tokens-openapi.yml
  format: yaml
  label: Modal Tokens and Administration API
  slug: modal-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/openapi/modal-tokens-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: modal.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: modal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 10:19:53 2026 GMT
  host: api.modal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modal Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modal, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Modal
provider_slug: modal
slug: modal-com-domain-security
source_filename: modal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.modal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 10:19:53 2026 GMT\n  hsts: null\ndomains:\n- domain: modal.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modal/refs/heads/main/security/modal-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Serverless
- GPU
- Cloud Compute
- AI Infrastructure
- Sandboxes
- Inference
- Training
- Batch Processing
- Python
- TypeScript
- Go
---
