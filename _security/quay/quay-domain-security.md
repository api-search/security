---
api_specs:
- filename: quay-build-api-openapi.yml
  format: yaml
  label: Quay Build API
  slug: quay-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-build-api-openapi.yml
- filename: quay-manifest-api-openapi.yml
  format: yaml
  label: Quay Manifest API
  slug: quay-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-manifest-api-openapi.yml
- filename: quay-organization-api-openapi.yml
  format: yaml
  label: Quay Organization API
  slug: quay-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-organization-api-openapi.yml
- filename: quay-permission-api-openapi.yml
  format: yaml
  label: Quay Permission API
  slug: quay-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-permission-api-openapi.yml
- filename: quay-repository-api-openapi.yml
  format: yaml
  label: Quay Repository API
  slug: quay-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-repository-api-openapi.yml
- filename: quay-robot-api-openapi.yml
  format: yaml
  label: Quay Robot API
  slug: quay-robot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-robot-api-openapi.yml
- filename: quay-security-api-openapi.yml
  format: yaml
  label: Quay Security API
  slug: quay-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-security-api-openapi.yml
- filename: quay-tag-api-openapi.yml
  format: yaml
  label: Quay Tag API
  slug: quay-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-tag-api-openapi.yml
- filename: quay-team-api-openapi.yml
  format: yaml
  label: Quay Team API
  slug: quay-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-team-api-openapi.yml
- filename: quay-user-api-openapi.yml
  format: yaml
  label: Quay User API
  slug: quay-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/openapi/quay-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quay.io
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: quay.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Quay
provider_slug: quay
slug: quay-domain-security
source_filename: quay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quay.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quay/refs/heads/main/security/quay-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Container Images
- Containers
- Red Hat
- Registry
- Security Scanning
---
