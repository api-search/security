---
api_specs:
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Documents API
  slug: scrive-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Templates API
  slug: scrive-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Signing API
  slug: scrive-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive e-ID Authentication API
  slug: scrive-eid-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Attachments API
  slug: scrive-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Callbacks API
  slug: scrive-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Access Control API
  slug: scrive-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:oi@scrive.com"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scrive.com
  spf: true
hosts:
- cert_expires: Aug 30 02:02:16 2026 GMT
  host: www.scrive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 12:09:49 2026 GMT
  host: apidocs.scrive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  4 23:59:59 2026 GMT
  host: scrive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scrive, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scrive
provider_slug: scrive
slug: scrive-domain-security
source_filename: scrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 02:02:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.scrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:09:49 2026 GMT\n  hsts: false\n- host: scrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: scrive.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:oi@scrive.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/security/scrive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Signature
- Electronic Signing
- Digital Identity
- e-ID
- BankID
- MitID
- Nordic
- Document Workflow
---
