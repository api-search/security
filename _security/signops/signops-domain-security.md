---
api_specs:
- filename: signops-approve-api-openapi.yml
  format: yaml
  label: SignOps Approve API
  slug: signops-approve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-approve-api-openapi.yml
- filename: signops-approve-sdk-api-openapi.yml
  format: yaml
  label: SignOps Approve SDK API
  slug: signops-approve-sdk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-approve-sdk-api-openapi.yml
- filename: signops-authenticator-api-openapi.yml
  format: yaml
  label: SignOps Authenticator API
  slug: signops-authenticator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-authenticator-api-openapi.yml
- filename: signops-devices-api-openapi.yml
  format: yaml
  label: SignOps Devices API
  slug: signops-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-devices-api-openapi.yml
- filename: signops-email-otp-api-openapi.yml
  format: yaml
  label: SignOps Email OTP API
  slug: signops-email-otp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-email-otp-api-openapi.yml
- filename: signops-inbox-api-openapi.yml
  format: yaml
  label: SignOps Inbox API
  slug: signops-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-inbox-api-openapi.yml
- filename: signops-live-activities-api-openapi.yml
  format: yaml
  label: SignOps Live Activities API
  slug: signops-live-activities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-live-activities-api-openapi.yml
- filename: signops-passkeys-api-openapi.yml
  format: yaml
  label: SignOps Passkeys API
  slug: signops-passkeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-passkeys-api-openapi.yml
- filename: signops-passkeys-browser-api-openapi.yml
  format: yaml
  label: SignOps Passkeys browser API
  slug: signops-passkeys-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-passkeys-browser-api-openapi.yml
- filename: signops-push-api-openapi.yml
  format: yaml
  label: SignOps Push API
  slug: signops-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-push-api-openapi.yml
- filename: signops-status-api-openapi.yml
  format: yaml
  label: SignOps Status API
  slug: signops-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-status-api-openapi.yml
- filename: signops-templates-api-openapi.yml
  format: yaml
  label: SignOps Templates API
  slug: signops-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-templates-api-openapi.yml
- filename: signops-topics-api-openapi.yml
  format: yaml
  label: SignOps Topics API
  slug: signops-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-topics-api-openapi.yml
- filename: signops-users-and-dpdp-api-openapi.yml
  format: yaml
  label: SignOps Users and DPDP API
  slug: signops-users-and-dpdp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-users-and-dpdp-api-openapi.yml
- filename: signops-verify-api-openapi.yml
  format: yaml
  label: SignOps Verify API
  slug: signops-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signops/openapi/signops-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: signops.dev
  spf: true
hosts:
- cert_expires: Jan 24 01:31:40 2027 GMT
  host: signops.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SignOps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SignOps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SignOps
provider_slug: signops
slug: signops-domain-security
source_filename: signops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signops.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 01:31:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: signops.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/signops/security/signops-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- OTP
- Push Notifications
- Passkeys
---
