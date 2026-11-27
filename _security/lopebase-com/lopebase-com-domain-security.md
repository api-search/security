---
api_specs:
- filename: lopebase-com-openapi-generated.yml
  format: yaml
  label: LopeBase API
  slug: lopebase-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lopebase-com/openapi/_ae-authored/lopebase-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lopebase.com
  spf: true
hosts:
- cert_expires: Dec 28 23:34:44 2026 GMT
  host: lopebase.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LopeBase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LopeBase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LopeBase
provider_slug: lopebase-com
slug: lopebase-com-domain-security
source_filename: lopebase-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lopebase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:34:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: lopebase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lopebase-com/security/lopebase-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software-as-a-Service
- Analytics
- SEO
---
