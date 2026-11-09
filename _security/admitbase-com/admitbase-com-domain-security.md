---
api_specs:
- filename: admitbase-com-openapi-generated.yml
  format: yaml
  label: AdmitBase API
  slug: admitbase-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/admitbase-com/openapi/_ae-authored/admitbase-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: admitbase.com
  spf: true
hosts:
- cert_expires: Jan 12 12:05:25 2027 GMT
  host: admitbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Admitbase Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdmitBase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AdmitBase
provider_slug: admitbase-com
slug: admitbase-com-domain-security
source_filename: admitbase-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: admitbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 12:05:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: admitbase.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/admitbase-com/security/admitbase-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Admissions
- Law
- Medical
- Dental
- Education
---
