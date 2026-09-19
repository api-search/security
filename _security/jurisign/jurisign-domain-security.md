---
api_specs:
- filename: jurisign-account-api-openapi.yml
  format: yaml
  label: JuriSign Account API
  slug: jurisign-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-account-api-openapi.yml
- filename: jurisign-authentication-api-openapi.yml
  format: yaml
  label: JuriSign Authentication API
  slug: jurisign-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-authentication-api-openapi.yml
- filename: jurisign-bulk-api-openapi.yml
  format: yaml
  label: JuriSign Bulk API
  slug: jurisign-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-bulk-api-openapi.yml
- filename: jurisign-documents-api-openapi.yml
  format: yaml
  label: JuriSign Documents API
  slug: jurisign-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-documents-api-openapi.yml
- filename: jurisign-public-forms-api-openapi.yml
  format: yaml
  label: JuriSign Public Forms API
  slug: jurisign-public-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-public-forms-api-openapi.yml
- filename: jurisign-sign-requests-api-openapi.yml
  format: yaml
  label: JuriSign Sign Requests API
  slug: jurisign-sign-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-sign-requests-api-openapi.yml
- filename: jurisign-templates-api-openapi.yml
  format: yaml
  label: JuriSign Templates API
  slug: jurisign-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-templates-api-openapi.yml
- filename: jurisign-webhooks-api-openapi.yml
  format: yaml
  label: JuriSign Webhooks API
  slug: jurisign-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jurisign.fr
  spf: true
hosts:
- cert_expires: Oct 28 13:12:28 2026 GMT
  host: www.jurisign.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 13:12:28 2026 GMT
  host: jurisign.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Jurisign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JuriSign, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JuriSign
provider_slug: jurisign
slug: jurisign-domain-security
source_filename: jurisign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jurisign.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 13:12:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: jurisign.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 13:12:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jurisign.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/security/jurisign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Electronic Signature
- E-Signature
- eIDAS
- Document Signing
- PDF
- Webhook
- OTP
- GDPR
- France
- Legal Tech
- Identity Verification
- Audit Trail
- data-residency-eu
---
