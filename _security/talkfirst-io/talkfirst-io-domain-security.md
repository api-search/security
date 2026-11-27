---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: talkfirst.io
  spf: false
hosts:
- cert_expires: Feb 23 23:00:55 2027 GMT
  host: talkfirst.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Talkfirst Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talkfirst, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Talkfirst
provider_slug: talkfirst-io
slug: talkfirst-io-domain-security
source_filename: talkfirst-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talkfirst.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:00:55 2027 GMT\n  hsts: false\ndomains:\n- domain: talkfirst.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/talkfirst-io/security/talkfirst-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Language Learning
- AI
- Voice Practice
- Education
- Speech Recognition
---
