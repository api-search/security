---
api_specs:
- filename: humanitec-openapi.yml
  format: yaml
  label: Humanitec Platform Orchestrator API
  slug: humanitec-platform-orchestrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanitec/refs/heads/main/openapi/humanitec-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: humanitec.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: humanitec.io
  spf: false
hosts:
- cert_expires: Aug 18 10:17:24 2026 GMT
  host: developer.humanitec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 13:31:06 2026 GMT
  host: humanitec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 07:25:55 2026 GMT
  host: api.humanitec.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humanitec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humanitec, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Humanitec
provider_slug: humanitec
slug: humanitec-domain-security
source_filename: humanitec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.humanitec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 10:17:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: humanitec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 13:31:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.humanitec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:25:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: humanitec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: humanitec.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanitec/refs/heads/main/security/humanitec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Deployments
- DevOps
- Internal Developer Platform
- Platform Engineering
- Platform Orchestrator
---
