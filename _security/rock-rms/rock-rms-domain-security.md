---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rockrms.com
  spf: false
hosts:
- cert_expires: Dec 13 17:31:01 2026 GMT
  host: rockrms.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rock RMS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rock RMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Rock RMS
provider_slug: rock-rms
slug: rock-rms-domain-security
source_filename: rock-rms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rockrms.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 17:31:01 2026 GMT\n  hsts: false\ndomains:\n- domain: rockrms.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/rock-rms/security/rock-rms-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Church Management
- Open Source
- Artificial Intelligence
- Cloud
---
