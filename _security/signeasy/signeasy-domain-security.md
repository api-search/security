---
api_specs:
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Envelopes API
  slug: signeasy-envelopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Originals API
  slug: signeasy-originals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Templates API
  slug: signeasy-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Embedded Signing API
  slug: signeasy-embedded-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Webhooks API
  slug: signeasy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Users API
  slug: signeasy-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: signeasy.com
  spf: true
hosts:
- cert_expires: Sep  5 05:42:52 2026 GMT
  host: signeasy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:02:27 2026 GMT
  host: docs.signeasy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 14 11:51:38 2027 GMT
  host: api.signeasy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signeasy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signeasy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Signeasy
provider_slug: signeasy
slug: signeasy-domain-security
source_filename: signeasy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signeasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:42:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.signeasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:02:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.signeasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 11:51:38 2027 GMT\n  hsts: null\ndomains:\n- domain: signeasy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/security/signeasy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eSignature
- Electronic Signature
- Documents
- Contract Management
- Embedded Signing
- Templates
- Webhooks
---
