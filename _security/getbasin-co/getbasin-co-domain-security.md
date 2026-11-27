---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getbasin.co
  spf: true
hosts:
- cert_expires: Jan  8 23:51:13 2027 GMT
  host: getbasin.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Basin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Basin
provider_slug: getbasin-co
slug: getbasin-co-domain-security
source_filename: getbasin-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getbasin.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:51:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getbasin.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getbasin-co/security/getbasin-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Assistant
- Automation
- Productivity
- Collaboration
---
