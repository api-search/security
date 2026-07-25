---
api_specs:
- filename: certifaction-account-api-openapi.yml
  format: yaml
  label: Certifaction Account API
  slug: certifaction-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifaction/refs/heads/main/openapi/certifaction-account-api-openapi.yml
- filename: certifaction-documents-api-openapi.yml
  format: yaml
  label: Certifaction Documents API
  slug: certifaction-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifaction/refs/heads/main/openapi/certifaction-documents-api-openapi.yml
- filename: certifaction-organization-api-openapi.yml
  format: yaml
  label: Certifaction Organization API
  slug: certifaction-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifaction/refs/heads/main/openapi/certifaction-organization-api-openapi.yml
- filename: certifaction-server-api-openapi.yml
  format: yaml
  label: Certifaction Server API
  slug: certifaction-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifaction/refs/heads/main/openapi/certifaction-server-api-openapi.yml
- filename: certifaction-signing-api-openapi.yml
  format: yaml
  label: Certifaction Signing API
  slug: certifaction-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifaction/refs/heads/main/openapi/certifaction-signing-api-openapi.yml
- filename: certifaction-teamspace-api-openapi.yml
  format: yaml
  label: Certifaction Teamspace API
  slug: certifaction-teamspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifaction/refs/heads/main/openapi/certifaction-teamspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: certifaction.com
  spf: true
hosts:
- cert_expires: Oct  4 23:35:48 2026 GMT
  host: certifaction.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Certifaction Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certifaction, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Certifaction
provider_slug: certifaction
slug: certifaction-domain-security
source_filename: certifaction-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: certifaction.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:35:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: certifaction.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certifaction/refs/heads/main/security/certifaction-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Enterprise Software
- Electronic Signature
- Digital Signature
- Document Signing
- Qualified Electronic Signature
- eIDAS
- Privacy
- Compliance
- Identity Verification
- Switzerland
---
