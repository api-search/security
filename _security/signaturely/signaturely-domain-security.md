---
api_specs:
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Signature Requests API
  slug: signaturely-signature-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Documents API
  slug: signaturely-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Templates API
  slug: signaturely-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Folders API
  slug: signaturely-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Team API
  slug: signaturely-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Webhooks API
  slug: signaturely-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely User API
  slug: signaturely-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: signaturely.com
  spf: true
hosts:
- cert_expires: Sep 24 15:15:26 2026 GMT
  host: signaturely.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: docs.signaturely.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.signaturely.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signaturely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signaturely, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Signaturely
provider_slug: signaturely
slug: signaturely-domain-security
source_filename: signaturely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signaturely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:15:26 2026 GMT\n  hsts: false\n- host: docs.signaturely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: false\n- host: api.signaturely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: signaturely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/security/signaturely-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Electronic Signature
- eSignature
- Document Signing
- E-Signature API
- Contracts
- Signature Requests
- SaaS
---
