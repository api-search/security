---
api_specs:
- filename: comarch-global-api-openapi.yml
  format: yaml
  label: Comarch Global API
  slug: comarch-global-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comarch/refs/heads/main/openapi/comarch-global-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: comarch.com
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.comarch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Comarch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comarch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Comarch
provider_slug: comarch
slug: comarch-domain-security
source_filename: comarch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.comarch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: comarch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comarch/refs/heads/main/security/comarch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IT
- Software
- Cloud
- Enterprise
- Global
---
