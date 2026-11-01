---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: operto.com
  spf: true
hosts:
- cert_expires: Jan  7 07:42:25 2027 GMT
  host: operto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Operto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Operto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Operto
provider_slug: operto
slug: operto-domain-security
source_filename: operto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: operto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 07:42:25 2027 GMT\n  hsts: false\ndomains:\n- domain: operto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://artifacts.apis.io/operto/security/operto-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hospitality
- Property Management
- Guest Experience
- Automation
---
