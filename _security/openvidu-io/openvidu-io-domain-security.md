---
api_specs:
- filename: openvidu-io-openapi-generated.yml
  format: yaml
  label: OpenVidu API
  slug: openvidu-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openvidu-io/openapi/_ae-authored/openvidu-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openvidu.io
  spf: true
hosts:
- cert_expires: Feb 15 19:57:18 2027 GMT
  host: openvidu.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenVidu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenVidu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenVidu
provider_slug: openvidu-io
slug: openvidu-io-domain-security
source_filename: openvidu-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openvidu.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 19:57:18 2027 GMT\n  hsts: false\ndomains:\n- domain: openvidu.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openvidu-io/security/openvidu-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video Conferencing
- WebRTC
- Open Source
- Real-Time
- Enterprise
---
