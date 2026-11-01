---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quitwithjones.com
  spf: true
hosts:
- cert_expires: Jan  5 01:47:01 2027 GMT
  host: quitwithjones.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quitwithjones Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jones, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jones
provider_slug: quitwithjones-com
slug: quitwithjones-com-domain-security
source_filename: quitwithjones-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quitwithjones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 01:47:01 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: quitwithjones.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/quitwithjones-com/security/quitwithjones-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Nicotine Replacement Therapy
- Health App
- FDA-approved
- Behavioral Support
---
