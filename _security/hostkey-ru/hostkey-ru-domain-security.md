---
api_specs:
- filename: hostkey-ru-openapi-generated.yml
  format: yaml
  label: HOSTKEY API
  slug: hostkey-ru-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hostkey-ru/openapi/_ae-authored/hostkey-ru-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hostkey.ru
  spf: true
hosts:
- cert_expires: Dec  9 08:10:24 2026 GMT
  host: hostkey.ru
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HOSTKEY Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HOSTKEY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HOSTKEY
provider_slug: hostkey-ru
slug: hostkey-ru-domain-security
source_filename: hostkey-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hostkey.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 08:10:24 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: hostkey.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hostkey-ru/security/hostkey-ru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hosting
- Cloud
- Servers
- Dedicated
- VPS
---
