---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flettu.is
  spf: true
hosts:
- cert_expires: Jan 14 20:55:11 2027 GMT
  host: flettu.is
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flettu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flettu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flettu
provider_slug: flettu-is
slug: flettu-is-domain-security
source_filename: flettu-is-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flettu.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 20:55:11 2027 GMT\n  hsts: false\ndomains:\n- domain: flettu.is\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flettu-is/security/flettu-is-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Iceland
- Data
- Finance
---
