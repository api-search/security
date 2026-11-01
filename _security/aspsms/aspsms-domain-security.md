---
api_specs:
- filename: aspsms-openapi-generated.yml
  format: yaml
  label: ASPSMS API
  slug: aspsms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspsms/openapi/_ae-authored/aspsms-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aspsms.com
  spf: true
hosts:
- cert_expires: Jan 20 07:39:58 2027 GMT
  host: www.aspsms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aspsms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ASPSMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ASPSMS
provider_slug: aspsms
slug: aspsms-domain-security
source_filename: aspsms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aspsms.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 07:39:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aspsms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/aspsms/security/aspsms-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- SMS
- Messaging
- API
- Communications
- Business
---
