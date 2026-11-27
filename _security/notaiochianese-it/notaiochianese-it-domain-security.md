---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: notaiochianese.it
  spf: true
hosts:
- cert_expires: Mar 20 18:03:15 2027 GMT
  host: notaiochianese.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Studio Notarile Chianese Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Studio Notarile Chianese, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Studio Notarile Chianese
provider_slug: notaiochianese-it
slug: notaiochianese-it-domain-security
source_filename: notaiochianese-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notaiochianese.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 18:03:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: notaiochianese.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/notaiochianese-it/security/notaiochianese-it-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notary
- Legal Services
- Italy
- Real Estate
- Family Law
---
