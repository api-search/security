---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: logiqc.com.au
  spf: true
hosts:
- cert_expires: Jan 14 11:22:32 2027 GMT
  host: www.logiqc.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Logiqc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logiqc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Logiqc
provider_slug: logiqc-com-au
slug: logiqc-com-au-domain-security
source_filename: logiqc-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.logiqc.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 11:22:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: logiqc.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/logiqc-com-au/security/logiqc-com-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Quality Management
- Healthcare
- Community Services
- Risk Management
---
