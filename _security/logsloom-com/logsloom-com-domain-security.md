---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: logsloom.com
  spf: true
hosts:
- cert_expires: Jan 31 14:14:50 2027 GMT
  host: logsloom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LogsLoom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LogsLoom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LogsLoom
provider_slug: logsloom-com
slug: logsloom-com-domain-security
source_filename: logsloom-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logsloom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 14:14:50 2027 GMT\n  hsts: false\ndomains:\n- domain: logsloom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/logsloom-com/security/logsloom-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Logging
- Software-as-a-Service
- Microservices
- Indie
---
