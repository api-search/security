---
api_specs:
- filename: cartoncloud-openapi-generated.yml
  format: yaml
  label: CartonCloud API
  slug: cartoncloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartoncloud/openapi/_ae-authored/cartoncloud-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cartoncloud.com
  spf: true
hosts:
- cert_expires: Jan 14 11:40:27 2027 GMT
  host: cartoncloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CartonCloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CartonCloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CartonCloud
provider_slug: cartoncloud
slug: cartoncloud-domain-security
source_filename: cartoncloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cartoncloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 11:40:27 2027 GMT\n  hsts: false\ndomains:\n- domain: cartoncloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cartoncloud/security/cartoncloud-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Logistics
- Software
- Warehouse Management
- Transportation
- Cloud
---
