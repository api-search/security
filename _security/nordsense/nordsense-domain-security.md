---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nordsense.com
  spf: true
hosts:
- cert_expires: Mar 25 23:59:59 2027 GMT
  host: nordsense.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nordsense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nordsense, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nordsense
provider_slug: nordsense
slug: nordsense-domain-security
source_filename: nordsense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nordsense.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nordsense.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nordsense/security/nordsense-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Sensors
- WasteManagement
- IoT
- DataInsights
---
