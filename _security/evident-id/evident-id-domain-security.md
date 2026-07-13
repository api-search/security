---
api_specs:
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Verification Requests API
  slug: evident-id-verification-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Attributes & Credentials API
  slug: evident-id-attributes-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Identity Assurance API
  slug: evident-id-identity-assurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Insurance & COI Verification API
  slug: evident-id-insurance-coi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Results API
  slug: evident-id-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Webhooks API
  slug: evident-id-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: evidentid.com
  spf: true
hosts:
- cert_expires: Aug 12 12:48:02 2026 GMT
  host: www.evidentid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 13:35:47 2026 GMT
  host: verify.api.evidentid.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 11 01:59:57 2026 GMT
  host: submit.api.evidentid.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Evident Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evident, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Evident
provider_slug: evident-id
slug: evident-id-domain-security
source_filename: evident-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evidentid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 12:48:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: verify.api.evidentid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 13:35:47 2026 GMT\n  hsts: null\n- host: submit.api.evidentid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 01:59:57 2026 GMT\n  hsts: null\ndomains:\n- domain: evidentid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/security/evident-id-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- Credential Verification
- Background Check
- Insurance Verification
- COI
---
