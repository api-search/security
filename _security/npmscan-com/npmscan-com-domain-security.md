---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: npmscan.com
  spf: false
hosts:
- cert_expires: Jan 23 06:19:03 2027 GMT
  host: npmscan.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NPMScan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NPMScan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: NPMScan
provider_slug: npmscan-com
slug: npmscan-com-domain-security
source_filename: npmscan-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: npmscan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 06:19:03 2027 GMT\n  hsts: null\ndomains:\n- domain: npmscan.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/npmscan-com/security/npmscan-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Security
- Supply Chain Security
- Malware Detection
- npm
- Threat Intelligence
- Developer Tools
---
