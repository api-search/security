---
api_specs:
- filename: encompass-developer-connect-openapi.yml
  format: yaml
  label: Encompass Developer Connect API
  slug: encompass-developer-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass-developer-connect/refs/heads/main/openapi/encompass-developer-connect-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: icemortgagetechnology.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elliemae.com
  spf: true
hosts:
- cert_expires: Oct  2 18:25:55 2026 GMT
  host: developer.icemortgagetechnology.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: api.elliemae.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Encompass Developer Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Encompass Developer Connect, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Encompass Developer Connect
provider_slug: encompass-developer-connect
slug: encompass-developer-connect-domain-security
source_filename: encompass-developer-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.icemortgagetechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:25:55 2026 GMT\n  hsts: null\n- host: api.elliemae.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: icemortgagetechnology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: elliemae.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encompass-developer-connect/refs/heads/main/security/encompass-developer-connect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Encompass
- ICE Mortgage Technology
- Loan Origination
- Lending
- Mortgage
- REST API
---
