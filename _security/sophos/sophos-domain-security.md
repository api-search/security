---
api_specs:
- filename: sophos-central-siem-openapi.yml
  format: yaml
  label: Sophos Central SIEM API
  slug: sophos-central-siem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sophos/refs/heads/main/openapi/sophos-central-siem-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sophos.com
  spf: true
hosts:
- cert_expires: Oct 12 15:36:01 2026 GMT
  host: developer.sophos.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  8 07:34:11 2026 GMT
  host: www.sophos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api1.central.sophos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sophos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sophos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sophos
provider_slug: sophos
slug: sophos-domain-security
source_filename: sophos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.sophos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 15:36:01 2026 GMT\n  hsts: null\n- host: www.sophos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 07:34:11 2026 GMT\n  hsts: null\n- host: api1.central.sophos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sophos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sophos/refs/heads/main/security/sophos-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Cybersecurity
- Endpoint Protection
- Security
- SIEM
- Threat Detection
- Incident Response
---
