---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: umoiq.com
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: retro.umoiq.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transport For United States Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for United States, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Transport for United States
provider_slug: transport-for-united-states
slug: transport-for-united-states-domain-security
source_filename: transport-for-united-states-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: retro.umoiq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: umoiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-united-states/refs/heads/main/security/transport-for-united-states-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Transportation
- Public APIs
---
