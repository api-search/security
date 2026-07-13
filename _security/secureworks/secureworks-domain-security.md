---
api_specs:
- filename: secureworks-taegis-xdr-openapi.yml
  format: yaml
  label: Secureworks Taegis XDR API
  slug: secureworks-taegis-xdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secureworks/refs/heads/main/openapi/secureworks-taegis-xdr-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: secureworks.com
  spf: true
hosts:
- cert_expires: Sep  8 07:34:11 2026 GMT
  host: www.secureworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: docs.taegis.secureworks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: api.ctpx.secureworks.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Secureworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Secureworks, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Secureworks
provider_slug: secureworks
slug: secureworks-domain-security
source_filename: secureworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.secureworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 07:34:11 2026 GMT\n  hsts: null\n- host: docs.taegis.secureworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ctpx.secureworks.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: secureworks.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secureworks/refs/heads/main/security/secureworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- XDR
- Threat Detection
- Security Operations
- Incident Response
- MDR
- Threat Intelligence
---
