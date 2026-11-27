---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jettracker.com.br
  spf: false
hosts:
- cert_expires: Feb  8 16:59:25 2027 GMT
  host: jettracker.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jet Tracker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jet Tracker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: Jet Tracker
provider_slug: jettracker-com-br
slug: jettracker-com-br-domain-security
source_filename: jettracker-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jettracker.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 16:59:25 2027 GMT\n  hsts: null\ndomains:\n- domain: jettracker.com.br\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/jettracker-com-br/security/jettracker-com-br-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Business Aviation
- Aircraft Registry
- Market Intelligence
- Sales CRM
- MRO
- Aviation Analytics
- Aircraft Listings
---
