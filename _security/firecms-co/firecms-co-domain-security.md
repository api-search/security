---
api_specs:
- filename: firecms-co-openapi-generated.yml
  format: yaml
  label: FireCMS API
  slug: firecms-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firecms-co/openapi/_ae-authored/firecms-co-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: firecms.co
  spf: true
hosts:
- cert_expires: Jan  8 17:50:33 2027 GMT
  host: firecms.co
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firecms Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FireCMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FireCMS
provider_slug: firecms-co
slug: firecms-co-domain-security
source_filename: firecms-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firecms.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 17:50:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: firecms.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/firecms-co/security/firecms-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- OpenSource
- CMS
- Firebase
- AdminPanel
---
