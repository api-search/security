---
api_specs:
- filename: tripeak-app-openapi-generated.yml
  format: yaml
  label: TriPeak API
  slug: tripeak-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripeak-app/openapi/_ae-authored/tripeak-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: tripeak.app
  spf: true
hosts:
- cert_expires: Jan 31 09:51:55 2027 GMT
  host: tripeak.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TriPeak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TriPeak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TriPeak
provider_slug: tripeak-app
slug: tripeak-app-domain-security
source_filename: tripeak-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tripeak.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 09:51:55 2027 GMT\n  hsts: false\ndomains:\n- domain: tripeak.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tripeak-app/security/tripeak-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
