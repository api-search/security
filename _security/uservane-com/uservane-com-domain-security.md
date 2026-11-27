---
api_specs:
- filename: uservane-com-privacy-api-openapi.yml
  format: yaml
  label: UserVane Privacy API
  slug: uservane-com-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uservane-com/openapi/uservane-com-privacy-api-openapi.yml
- filename: uservane-com-public-sdk-api-openapi.yml
  format: yaml
  label: UserVane Public SDK API
  slug: uservane-com-public-sdk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uservane-com/openapi/uservane-com-public-sdk-api-openapi.yml
- filename: uservane-com-secret-sdk-api-openapi.yml
  format: yaml
  label: UserVane Secret SDK API
  slug: uservane-com-secret-sdk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uservane-com/openapi/uservane-com-secret-sdk-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: uservane.com
  spf: true
hosts:
- cert_expires: Feb 21 00:17:26 2027 GMT
  host: uservane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: UserVane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UserVane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UserVane
provider_slug: uservane-com
slug: uservane-com-domain-security
source_filename: uservane-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uservane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 00:17:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uservane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/uservane-com/security/uservane-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- Survey
- AI
- CustomerFeedback
---
