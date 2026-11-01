---
api_specs:
- filename: frigate-openapi-generated.yml
  format: yaml
  label: Frigate NVR API
  slug: frigate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frigate/openapi/_ae-authored/frigate-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: frigate.video
  spf: true
hosts:
- cert_expires: May 13 14:01:53 2027 GMT
  host: frigate.video
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Frigate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frigate NVR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Frigate NVR
provider_slug: frigate
slug: frigate-domain-security
source_filename: frigate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frigate.video\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 13 14:01:53 2027 GMT\n  hsts: false\ndomains:\n- domain: frigate.video\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/frigate/security/frigate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Surveillance
- OpenSource
- AI
---
