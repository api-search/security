---
api_specs:
- filename: ovms-openapi-generated.yml
  format: yaml
  label: Open Vehicle Monitoring System (self-hosted) API
  slug: ovms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ovms/openapi/_ae-authored/ovms-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openvehicles.com
  spf: true
hosts:
- cert_expires: Jan  8 11:42:14 2027 GMT
  host: openvehicles.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ovms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Vehicle Monitoring System (self-hosted), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Vehicle Monitoring System (self-hosted)
provider_slug: ovms
slug: ovms-domain-security
source_filename: ovms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openvehicles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 11:42:14 2027 GMT\n  hsts: false\ndomains:\n- domain: openvehicles.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ovms/security/ovms-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Telematics
- Electric Vehicles
- Open Source
- IoT
- Automotive
---
