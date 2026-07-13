---
api_specs:
- filename: dxc-developer-central-api-openapi.yml
  format: yaml
  label: DXC Developer Central API
  slug: developer-central-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dxc-technology/refs/heads/main/openapi/dxc-developer-central-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dxc.com
  spf: true
hosts:
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: dxc.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: developer.dxc.com
  https: false
kind: domain-security
layout: security
method: probed
name: Dxc Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DXC Technology, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DXC Technology
provider_slug: dxc-technology
slug: dxc-technology-domain-security
source_filename: dxc-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dxc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.dxc.com\n  https: false\ndomains:\n- domain: dxc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dxc-technology/refs/heads/main/security/dxc-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IT Services
- Enterprise
- Platform
- Integration
---
