---
api_specs:
- filename: cirrus-identity-log-api-openapi.json
  format: json
  label: Cirrus Identity Log API
  slug: cirrus-identity-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cirrus-identity/refs/heads/main/openapi/cirrus-identity-log-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cirrusidentity.com
  spf: true
hosts:
- cert_expires: Sep 15 23:41:13 2026 GMT
  host: cirrusidentity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cirrus Identity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cirrus Identity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cirrus Identity
provider_slug: cirrus-identity
slug: cirrus-identity-domain-security
source_filename: cirrus-identity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cirrusidentity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:41:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cirrusidentity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cirrus-identity/refs/heads/main/security/cirrus-identity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity
- Authentication
- Single Sign-On
- SAML
- OIDC
- Higher Education
- Identity Management
- Federation
- Logs
---
