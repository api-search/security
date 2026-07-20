---
api_specs:
- filename: levelblue-usm-anywhere-openapi.yml
  format: yaml
  label: USM Anywhere API
  slug: usm-anywhere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levelblue/refs/heads/main/openapi/levelblue-usm-anywhere-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: levelblue.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alienvault.cloud
  spf: true
hosts:
- cert_expires: Aug 31 00:38:30 2026 GMT
  host: docs.levelblue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: your-subdomain.alienvault.cloud
  https: false
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: otx.alienvault.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Levelblue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LevelBlue, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LevelBlue
provider_slug: levelblue
slug: levelblue-domain-security
source_filename: levelblue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.levelblue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 00:38:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-subdomain.alienvault.cloud\n  https: false\n- host: otx.alienvault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: levelblue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: alienvault.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levelblue/refs/heads/main/security/levelblue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Cybersecurity
- Security
- Threat Intelligence
- Managed Security
- SIEM
- Threat Detection
- Incident Response
- Compliance
---
