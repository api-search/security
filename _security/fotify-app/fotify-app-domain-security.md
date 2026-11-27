---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fotify.app
  spf: true
hosts:
- cert_expires: Jan 30 16:31:18 2027 GMT
  host: fotify.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fotify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fotify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fotify
provider_slug: fotify-app
slug: fotify-app-domain-security
source_filename: fotify-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fotify.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 16:31:18 2027 GMT\n  hsts: false\ndomains:\n- domain: fotify.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fotify-app/security/fotify-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Photo Sharing
- Event Management
- DigitalInvitations
- Artificial Intelligence
---
