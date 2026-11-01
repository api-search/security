---
api_specs:
- filename: accompany-openapi-generated.yml
  format: yaml
  label: Accompany API
  slug: accompany-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accompany/openapi/_ae-authored/accompany-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: accompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zendesk.com
  spf: true
hosts:
- cert_expires: Apr  1 23:59:59 2027 GMT
  host: www.accompany.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 13:46:56 2026 GMT
  host: developer.zendesk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Accompany Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accompany, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Accompany
provider_slug: accompany
slug: accompany-domain-security
source_filename: accompany-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.zendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 13:46:56 2026 GMT\n  hsts: false\ndomains:\n- domain: accompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: zendesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/accompany/security/accompany-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Relationship Intelligence
- Sales Intelligence
- Acquired
- Defunct
---
