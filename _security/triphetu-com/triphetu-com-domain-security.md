---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: triphetu.com
  spf: true
hosts:
- cert_expires: Jan 27 08:02:31 2027 GMT
  host: triphetu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Triphetu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Triphetu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Triphetu
provider_slug: triphetu-com
slug: triphetu-com-domain-security
source_filename: triphetu-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: triphetu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 08:02:31 2027 GMT\n  hsts: false\ndomains:\n- domain: triphetu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/triphetu-com/security/triphetu-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Trip Planning
- Group Travel
- Live Map
- AI Assistant
- Travel App
---
