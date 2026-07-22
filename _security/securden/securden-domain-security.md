---
api_specs:
- filename: securden-password-retrieval-openapi.yml
  format: yaml
  label: Securden Password Retrieval API
  slug: securden-password-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securden/refs/heads/main/openapi/securden-password-retrieval-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: securden.com
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: www.securden.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Securden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Securden, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Securden
provider_slug: securden
slug: securden-domain-security
source_filename: securden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.securden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: securden.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securden/refs/heads/main/security/securden-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Identity
- Security
- Privileged Access Management
- Password Management
- Secrets Management
- Endpoint Security
- DevOps
- AI Agent Security
---
