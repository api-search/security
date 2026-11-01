---
api_specs:
- filename: openhab-configuration-openapi-generated.yml
  format: yaml
  label: openHAB Configuration Overview API
  slug: configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openhab/openapi/_ae-authored/openhab-configuration-openapi-generated.yml
- filename: openhab-installation-openapi-generated.yml
  format: yaml
  label: openHAB Installation Overview API
  slug: installation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openhab/openapi/_ae-authored/openhab-installation-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openhab.org
  spf: true
hosts:
- cert_expires: Dec 22 13:13:48 2026 GMT
  host: openhab.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openhab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for openHAB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: openHAB
provider_slug: openhab
slug: openhab-domain-security
source_filename: openhab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openhab.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 13:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openhab.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openhab/security/openhab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Home Automation
- Open Source
- IoT
- Smart Home
- Vendor Agnostic
---
