---
api_specs:
- filename: sovos-configurations-api-openapi.yml
  format: yaml
  label: Sovos Configurations API
  slug: sovos-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovos/refs/heads/main/openapi/sovos-configurations-api-openapi.yml
- filename: sovos-documents-api-openapi.yml
  format: yaml
  label: Sovos Documents API
  slug: sovos-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovos/refs/heads/main/openapi/sovos-documents-api-openapi.yml
- filename: sovos-notifications-api-openapi.yml
  format: yaml
  label: Sovos Notifications API
  slug: sovos-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovos/refs/heads/main/openapi/sovos-notifications-api-openapi.yml
- filename: sovos-oauth-api-openapi.yml
  format: yaml
  label: Sovos OAuth API
  slug: sovos-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovos/refs/heads/main/openapi/sovos-oauth-api-openapi.yml
- filename: sovos-taxid-checks-api-openapi.yml
  format: yaml
  label: Sovos Taxid Checks API
  slug: sovos-taxid-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sovos/refs/heads/main/openapi/sovos-taxid-checks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sovos.com
  spf: true
hosts:
- cert_expires: Jan  6 00:45:43 2027 GMT
  host: sovos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sovos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sovos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sovos
provider_slug: sovos
slug: sovos-domain-security
source_filename: sovos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sovos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 00:45:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sovos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sovos/refs/heads/main/security/sovos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tax
- Compliance
- Cloud
- Global
---
