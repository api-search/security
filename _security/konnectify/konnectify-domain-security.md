---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: konnectify.co
  spf: true
hosts:
- cert_expires: May  1 23:59:59 2027 GMT
  host: konnectify.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Konnectify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Konnectify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Konnectify
provider_slug: konnectify
slug: konnectify-domain-security
source_filename: konnectify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konnectify.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: konnectify.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/konnectify/security/konnectify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Integration Platform
- Artificial Intelligence
- Automation
- Software-as-a-Service
- Low-Code
---
