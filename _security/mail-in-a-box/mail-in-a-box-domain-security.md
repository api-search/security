---
api_specs:
- filename: mail-in-a-box-dns-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box DNS API
  slug: mail-in-a-box-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-dns-api-openapi.yml
- filename: mail-in-a-box-mail-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box Mail API
  slug: mail-in-a-box-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-mail-api-openapi.yml
- filename: mail-in-a-box-mfa-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box MFA API
  slug: mail-in-a-box-mfa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-mfa-api-openapi.yml
- filename: mail-in-a-box-ssl-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box SSL API
  slug: mail-in-a-box-ssl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-ssl-api-openapi.yml
- filename: mail-in-a-box-system-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box System API
  slug: mail-in-a-box-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-system-api-openapi.yml
- filename: mail-in-a-box-user-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box User API
  slug: mail-in-a-box-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-user-api-openapi.yml
- filename: mail-in-a-box-web-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box Web API
  slug: mail-in-a-box-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mailinabox.email
  spf: true
hosts:
- cert_expires: Jan  9 04:41:00 2027 GMT
  host: mailinabox.email
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mail In A Box Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mail-in-a-Box, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mail-in-a-Box
provider_slug: mail-in-a-box
slug: mail-in-a-box-domain-security
source_filename: mail-in-a-box-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailinabox.email\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 04:41:00 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: mailinabox.email\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mail-in-a-box/security/mail-in-a-box-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email
- Self-hosted
- Open-source
- Automation
- Privacy
---
