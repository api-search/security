---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reform.app
  spf: true
hosts:
- cert_expires: Aug 22 08:56:09 2026 GMT
  host: www.reform.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.reform.app
  https: false
kind: domain-security
layout: security
method: probed
name: Reform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reform, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reform
provider_slug: reform
slug: reform-domain-security
source_filename: reform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reform.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:56:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.reform.app\n  https: false\ndomains:\n- domain: reform.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reform/refs/heads/main/security/reform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forms
- Form Builder
- Lead Generation
- Headless Forms
- Webhooks
- No-Code
- Integrations
- CRM
---
