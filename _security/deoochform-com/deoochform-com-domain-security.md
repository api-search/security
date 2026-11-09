---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deoochform.com
  spf: true
hosts:
- cert_expires: Jan 12 10:03:57 2027 GMT
  host: deoochform.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deoochform Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deoochform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Deoochform
provider_slug: deoochform-com
slug: deoochform-com-domain-security
source_filename: deoochform-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deoochform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 10:03:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deoochform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/deoochform-com/security/deoochform-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Forms
- Form Builder
- Surveys
- Artificial Intelligence
- MCP
- Payments
- Webhook
- No-Code
---
