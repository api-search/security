---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: iisrescue.com
  spf: true
hosts:
- cert_expires: Feb  3 13:26:31 2027 GMT
  host: iisrescue.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IIS Rescue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IIS Rescue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: IIS Rescue
provider_slug: iisrescue-com
slug: iisrescue-com-domain-security
source_filename: iisrescue-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iisrescue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 13:26:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iisrescue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/iisrescue-com/security/iisrescue-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Migration
- IIS
- Cloud
- Legacy
- Small Business
---
