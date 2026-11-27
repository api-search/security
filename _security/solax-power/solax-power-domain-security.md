---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: solaxcloud.com
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: solaxcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SolaX Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SolaX Cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SolaX Cloud
provider_slug: solax-power
slug: solax-power-domain-security
source_filename: solax-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solaxcloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: solaxcloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/solax-power/security/solax-power-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Solar
- Energy
- Monitoring
- IoT
- Cloud
---
