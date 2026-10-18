---
api_specs:
- filename: esendex-credential-management-api-openapi.yml
  format: yaml
  label: Esendex Credential Management API
  slug: esendex-credential-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/openapi/esendex-credential-management-api-openapi.yml
- filename: esendex-message-dispatcher-api-openapi.yml
  format: yaml
  label: Esendex Message Dispatcher API
  slug: esendex-message-dispatcher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/openapi/esendex-message-dispatcher-api-openapi.yml
- filename: esendex-message-headers-api-openapi.yml
  format: yaml
  label: Esendex Message Headers API
  slug: esendex-message-headers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/openapi/esendex-message-headers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: esendex.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: www.esendex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Esendex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Esendex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Esendex
provider_slug: esendex
slug: esendex-domain-security
source_filename: esendex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esendex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: esendex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esendex/refs/heads/main/security/esendex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SMS
- Messaging
- Communications
- Business
---
