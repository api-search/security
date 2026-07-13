---
api_specs:
- filename: acquia-cloud-openapi.yml
  format: yaml
  label: Acquia Cloud API
  slug: acquia-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-cloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: acquia.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: dev.acquia.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 19 23:59:59 2026 GMT
  host: cloudapi-docs.acquia.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acquia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acquia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Acquia
provider_slug: acquia
slug: acquia-domain-security
source_filename: acquia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.acquia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n- host: cloudapi-docs.acquia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: acquia.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/security/acquia-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Content
- Experience
---
