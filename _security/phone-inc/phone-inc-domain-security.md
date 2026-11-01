---
api_specs:
- filename: phone-inc-openapi-generated.yml
  format: yaml
  label: Phone Inc API
  slug: phone-inc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phone-inc/openapi/_ae-authored/phone-inc-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: phone.inc
  spf: true
hosts:
- cert_expires: Dec 25 13:47:23 2026 GMT
  host: www.phone.inc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Phone Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phone Inc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Phone Inc
provider_slug: phone-inc
slug: phone-inc-domain-security
source_filename: phone-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.phone.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 13:47:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: phone.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/phone-inc/security/phone-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Communications
- Cloud
- Business
- API
---
