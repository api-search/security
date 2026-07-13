---
api_specs:
- filename: modal-labs-openapi.yml
  format: yaml
  label: Modal Web Endpoints
  slug: modal-labs-web-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-labs/refs/heads/main/openapi/modal-labs-openapi.yml
- filename: modal-labs-openapi.yml
  format: yaml
  label: Modal Sandboxes
  slug: modal-labs-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-labs/refs/heads/main/openapi/modal-labs-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: modal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: modal.run
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: modal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: <workspace>--<app>-<function>.modal.run
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''<workspace>'
kind: domain-security
layout: security
method: probed
name: Modal Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modal, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Modal
provider_slug: modal-labs
slug: modal-labs-domain-security
source_filename: modal-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: <workspace>--<app>-<function>.modal.run\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''<workspace>'\n  hsts: null\ndomains:\n- domain: modal.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: modal.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modal-labs/refs/heads/main/security/modal-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Serverless
- Compute
- GPU
- AI Infrastructure
- Sandboxes
- Infrastructure as Code
---
