---
api_specs:
- filename: homenet-openapi-generated.yml
  format: yaml
  label: HomeNet (Cox Automotive) API
  slug: homenet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homenet/openapi/_ae-authored/homenet-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: homenetauto.com
  spf: true
hosts:
- cert_expires: Jan 27 10:15:36 2027 GMT
  host: homenetauto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HomeNet (Cox Automotive) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HomeNet (Cox Automotive), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HomeNet (Cox Automotive)
provider_slug: homenet
slug: homenet-domain-security
source_filename: homenet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homenetauto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 10:15:36 2027 GMT\n  hsts: false\ndomains:\n- domain: homenetauto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/homenet/security/homenet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Digital Merchandising
- Dealer Solutions
- Cox Automotive
---
