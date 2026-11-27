---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: formbuilder.com
  spf: true
hosts:
- cert_expires: Jan 24 11:34:58 2027 GMT
  host: formbuilder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FormBuilder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FormBuilder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FormBuilder
provider_slug: formbuilder-com
slug: formbuilder-com-domain-security
source_filename: formbuilder-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formbuilder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 11:34:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: formbuilder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/formbuilder-com/security/formbuilder-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Form Builder
- Online Forms
- No-Code
- Artificial Intelligence
---
