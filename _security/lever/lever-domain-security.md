---
api_specs:
- filename: lever-openapi.yml
  format: yaml
  label: Lever Opportunities API
  slug: lever-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever/refs/heads/main/openapi/lever-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lever.co
  spf: true
hosts:
- cert_expires: Sep 27 08:49:28 2026 GMT
  host: www.lever.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: api.lever.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lever Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lever, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lever
provider_slug: lever
slug: lever-domain-security
source_filename: lever-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lever.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 08:49:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lever.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lever.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lever/refs/heads/main/security/lever-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- ATS
- Recruiting
- Talent Acquisition
- SaaS
---
