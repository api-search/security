---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uplinkswitch.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uplinkswitch.com
  spf: true
hosts:
- cert_expires: Jan 17 00:39:13 2027 GMT
  host: uplinkswitch.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 04:15:52 2027 GMT
  host: api.uplinkswitch.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Uplinkswitch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UplinkSwitch, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: UplinkSwitch
provider_slug: uplinkswitch
slug: uplinkswitch-domain-security
source_filename: uplinkswitch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uplinkswitch.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 00:39:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.uplinkswitch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 04:15:52 2027 GMT\n  hsts: null\ndomains:\n- domain: uplinkswitch.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: uplinkswitch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/uplinkswitch/security/uplinkswitch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Gateway
- Reseller
- Platform
---
