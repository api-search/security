---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coghorizon.com
  spf: true
hosts:
- cert_expires: Jan 11 07:20:26 2027 GMT
  host: coghorizon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coghorizon Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognitive Horizon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cognitive Horizon
provider_slug: coghorizon-com
slug: coghorizon-com-domain-security
source_filename: coghorizon-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coghorizon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 07:20:26 2027 GMT\n  hsts: false\ndomains:\n- domain: coghorizon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/coghorizon-com/security/coghorizon-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical
- Knowledge
- Artificial Intelligence
- Healthcare
- Consulting
---
