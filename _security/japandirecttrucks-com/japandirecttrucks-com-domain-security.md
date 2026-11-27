---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: japandirecttrucks.com
  spf: true
hosts:
- cert_expires: Dec 22 00:22:46 2026 GMT
  host: japandirecttrucks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Japan Direct Trucks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Japan Direct Trucks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Japan Direct Trucks
provider_slug: japandirecttrucks-com
slug: japandirecttrucks-com-domain-security
source_filename: japandirecttrucks-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: japandirecttrucks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 00:22:46 2026 GMT\n  hsts: false\ndomains:\n- domain: japandirecttrucks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/japandirecttrucks-com/security/japandirecttrucks-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Export
- Trucks
- Japan
---
