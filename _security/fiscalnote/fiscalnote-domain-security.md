---
api_specs:
- filename: fiscalnote-policynote-openapi.yml
  format: yaml
  label: FiscalNote PolicyNote API
  slug: policynote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-policynote-openapi.yml
- filename: fiscalnote-appdata-openapi.yml
  format: yaml
  label: FiscalNote AppData API
  slug: appdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-appdata-openapi.yml
- filename: fiscalnote-people-openapi.yml
  format: yaml
  label: FiscalNote People API
  slug: people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-people-openapi.yml
- filename: fiscalnote-organization-openapi.yml
  format: yaml
  label: FiscalNote Organization API
  slug: organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-organization-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fiscalnote.com
  spf: true
hosts:
- cert_expires: Aug 26 22:29:30 2026 GMT
  host: fiscalnote.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: apidocs.fiscalnote.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''apidocs.fis'
- host: api.fiscalnote.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fiscalnote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FiscalNote, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FiscalNote
provider_slug: fiscalnote
slug: fiscalnote-domain-security
source_filename: fiscalnote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fiscalnote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 22:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: apidocs.fiscalnote.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''apidocs.fis'\n  hsts: null\n- host: api.fiscalnote.com\n  https: false\ndomains:\n- domain: fiscalnote.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/security/fiscalnote-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Legislation
- Policy
- Political Intelligence
- Regulation
---
