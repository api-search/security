---
api_specs:
- filename: mailprobe-dev-account-api-openapi.yml
  format: yaml
  label: mailprobe-dev Account API
  slug: mailprobe-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailprobe-dev/openapi/mailprobe-dev-account-api-openapi.yml
- filename: mailprobe-dev-verification-api-openapi.yml
  format: yaml
  label: mailprobe-dev Verification API
  slug: mailprobe-dev-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailprobe-dev/openapi/mailprobe-dev-verification-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mailprobe.dev
  spf: true
hosts:
- cert_expires: Dec 22 03:43:12 2026 GMT
  host: mailprobe.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailprobe Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mailprobe-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: mailprobe-dev
provider_slug: mailprobe-dev
slug: mailprobe-dev-domain-security
source_filename: mailprobe-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailprobe.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 03:43:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailprobe.dev\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mailprobe-dev/security/mailprobe-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email Verification
- API
- Real-time
- Developer Tools
---
