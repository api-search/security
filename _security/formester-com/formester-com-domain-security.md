---
api_specs:
- filename: formester-com-openapi-generated.yml
  format: yaml
  label: Formester API
  slug: formester-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formester-com/openapi/_ae-authored/formester-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: formester.com
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: formester.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Formester Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formester, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Formester
provider_slug: formester-com
slug: formester-com-domain-security
source_filename: formester-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formester.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: formester.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/formester-com/security/formester-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Form Builder
- Workflow Automation
- No-Code
- AI-enhanced
- Free
---
