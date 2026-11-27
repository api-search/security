---
api_specs:
- filename: google-workspace-allowlisteddomains-api-openapi.yml
  format: yaml
  label: Google Workspace Allowlisted Domains API
  slug: google-workspace-allowlisteddomains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-allowlisteddomains-api-openapi.yml
- filename: google-workspace-customerlicense-api-openapi.yml
  format: yaml
  label: Google Workspace Customer License API
  slug: google-workspace-customerlicense-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-customerlicense-api-openapi.yml
- filename: google-workspace-customers-api-openapi.yml
  format: yaml
  label: Google Workspace Customers API
  slug: google-workspace-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-customers-api-openapi.yml
- filename: google-workspace-devices-api-openapi.yml
  format: yaml
  label: Google Workspace Devices API
  slug: google-workspace-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-devices-api-openapi.yml
- filename: google-workspace-groups-api-openapi.yml
  format: yaml
  label: Google Workspace Groups API
  slug: google-workspace-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-groups-api-openapi.yml
- filename: google-workspace-inboundoidcssoprofiles-api-openapi.yml
  format: yaml
  label: Google Workspace Inbound Oidc SSO Profiles API
  slug: google-workspace-inboundoidcssoprofiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-inboundoidcssoprofiles-api-openapi.yml
- filename: google-workspace-inboundsamlssoprofiles-api-openapi.yml
  format: yaml
  label: Google Workspace Inbound Saml SSO Profiles API
  slug: google-workspace-inboundsamlssoprofiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-inboundsamlssoprofiles-api-openapi.yml
- filename: google-workspace-inboundssoassignments-api-openapi.yml
  format: yaml
  label: Google Workspace Inbound SSO Assignments API
  slug: google-workspace-inboundssoassignments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-inboundssoassignments-api-openapi.yml
- filename: google-workspace-operations-api-openapi.yml
  format: yaml
  label: Google Workspace Operations API
  slug: google-workspace-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-operations-api-openapi.yml
- filename: google-workspace-policies-api-openapi.yml
  format: yaml
  label: Google Workspace Policies API
  slug: google-workspace-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-policies-api-openapi.yml
- filename: google-workspace-subscriptions-api-openapi.yml
  format: yaml
  label: Google Workspace Subscriptions API
  slug: google-workspace-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-subscriptions-api-openapi.yml
- filename: google-workspace-userlicense-api-openapi.yml
  format: yaml
  label: Google Workspace User License API
  slug: google-workspace-userlicense-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-workspace/openapi/google-workspace-userlicense-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: workspace.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: gmail.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Workspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Workspace, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Workspace
provider_slug: google-workspace
slug: google-workspace-domain-security
source_filename: google-workspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workspace.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: gmail.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-workspace/security/google-workspace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Calendar
- Collaboration
- Email
- Productivity
- Storage
- Video Conferencing
- Google Workspace
---
