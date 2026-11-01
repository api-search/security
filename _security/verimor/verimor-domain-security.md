---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verimor.com.tr
  spf: true
hosts:
- cert_expires: Jan 20 12:45:40 2027 GMT
  host: verimor.com.tr
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Verimor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verimor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verimor
provider_slug: verimor
slug: verimor-domain-security
source_filename: verimor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verimor.com.tr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 12:45:40 2027 GMT\n  hsts: null\ndomains:\n- domain: verimor.com.tr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/verimor/security/verimor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SMS
- WhatsApp
- API
---
