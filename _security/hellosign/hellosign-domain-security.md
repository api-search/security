---
api_specs:
- filename: hellosign-account-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Account API
  slug: hellosign-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-account-api-openapi.yml
- filename: hellosign-api-app-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Api App API
  slug: hellosign-api-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-api-app-api-openapi.yml
- filename: hellosign-bulk-send-job-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Bulk Send Job API
  slug: hellosign-bulk-send-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-bulk-send-job-api-openapi.yml
- filename: hellosign-embedded-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Embedded API
  slug: hellosign-embedded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-embedded-api-openapi.yml
- filename: hellosign-fax-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Fax API
  slug: hellosign-fax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-fax-api-openapi.yml
- filename: hellosign-fax-line-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Fax Line API
  slug: hellosign-fax-line-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-fax-line-api-openapi.yml
- filename: hellosign-oauth-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) OAuth API
  slug: hellosign-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-oauth-api-openapi.yml
- filename: hellosign-report-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Report API
  slug: hellosign-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-report-api-openapi.yml
- filename: hellosign-signature-request-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Signature Request API
  slug: hellosign-signature-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-signature-request-api-openapi.yml
- filename: hellosign-team-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Team API
  slug: hellosign-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-team-api-openapi.yml
- filename: hellosign-template-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Template API
  slug: hellosign-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-template-api-openapi.yml
- filename: hellosign-unclaimed-draft-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Unclaimed Draft API
  slug: hellosign-unclaimed-draft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-unclaimed-draft-api-openapi.yml
- filename: hellosign-callbacks-and-events-api-openapi.yml
  format: yaml
  label: Dropbox Sign (HelloSign) Callbacks and Events API
  slug: hellosign-callbacks-and-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-callbacks-and-events-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hellosign.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.hellosign.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hellosign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dropbox Sign (HelloSign), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dropbox Sign (HelloSign)
provider_slug: hellosign
slug: hellosign-domain-security
source_filename: hellosign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.hellosign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hellosign.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/security/hellosign-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- eSignature
- Electronic Signatures
- Documents
- Digital Agreements
- Signature Workflow
- Embedded Signing
- Compliance
---
