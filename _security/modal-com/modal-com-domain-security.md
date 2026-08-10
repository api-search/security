---
api_specs:
- filename: modal-com-apps-api-openapi.yml
  format: yaml
  label: Modal Apps API
  slug: modal-com-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-apps-api-openapi.yml
- filename: modal-com-dicts-api-openapi.yml
  format: yaml
  label: Modal Dicts API
  slug: modal-com-dicts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-dicts-api-openapi.yml
- filename: modal-com-environments-api-openapi.yml
  format: yaml
  label: Modal Environments API
  slug: modal-com-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-environments-api-openapi.yml
- filename: modal-com-execution-api-openapi.yml
  format: yaml
  label: Modal Execution API
  slug: modal-com-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-execution-api-openapi.yml
- filename: modal-com-files-api-openapi.yml
  format: yaml
  label: Modal Files API
  slug: modal-com-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-files-api-openapi.yml
- filename: modal-com-filesystem-api-openapi.yml
  format: yaml
  label: Modal Filesystem API
  slug: modal-com-filesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-filesystem-api-openapi.yml
- filename: modal-com-functions-api-openapi.yml
  format: yaml
  label: Modal Functions API
  slug: modal-com-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-functions-api-openapi.yml
- filename: modal-com-images-api-openapi.yml
  format: yaml
  label: Modal Images API
  slug: modal-com-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-images-api-openapi.yml
- filename: modal-com-invocations-api-openapi.yml
  format: yaml
  label: Modal Invocations API
  slug: modal-com-invocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-invocations-api-openapi.yml
- filename: modal-com-queues-api-openapi.yml
  format: yaml
  label: Modal Queues API
  slug: modal-com-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-queues-api-openapi.yml
- filename: modal-com-sandboxes-api-openapi.yml
  format: yaml
  label: Modal Sandboxes API
  slug: modal-com-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-sandboxes-api-openapi.yml
- filename: modal-com-schedules-api-openapi.yml
  format: yaml
  label: Modal Schedules API
  slug: modal-com-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-schedules-api-openapi.yml
- filename: modal-com-secrets-api-openapi.yml
  format: yaml
  label: Modal Secrets API
  slug: modal-com-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-secrets-api-openapi.yml
- filename: modal-com-tokens-api-openapi.yml
  format: yaml
  label: Modal Tokens API
  slug: modal-com-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-tokens-api-openapi.yml
- filename: modal-com-volumes-api-openapi.yml
  format: yaml
  label: Modal Volumes API
  slug: modal-com-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-volumes-api-openapi.yml
- filename: modal-com-webendpoints-api-openapi.yml
  format: yaml
  label: Modal WebEndpoints API
  slug: modal-com-webendpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-webendpoints-api-openapi.yml
- filename: modal-com-workspaces-api-openapi.yml
  format: yaml
  label: Modal Workspaces API
  slug: modal-com-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/openapi/modal-com-workspaces-api-openapi.yml
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
provider_slug: modal-com
slug: modal-com-domain-security
source_filename: modal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.modal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 10:19:53 2026 GMT\n  hsts: null\ndomains:\n- domain: modal.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modal-com/refs/heads/main/security/modal-com-domain-security.yml
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
