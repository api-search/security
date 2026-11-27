---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: expatliving.it
  spf: true
hosts:
- cert_expires: Feb  3 22:00:23 2027 GMT
  host: expatliving.it
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Expat Living Italy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expat Living Italy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Expat Living Italy
provider_slug: expatliving-it
slug: expatliving-it-domain-security
source_filename: expatliving-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: expatliving.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 22:00:23 2027 GMT\n  hsts: null\ndomains:\n- domain: expatliving.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/expatliving-it/security/expatliving-it-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- Expats
- Retirement
- Open Data
- Italy
---
