---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: stackpath.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.stackpath.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stackpath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StackPath, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: StackPath
provider_slug: stackpath
slug: stackpath-domain-security
source_filename: stackpath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stackpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: stackpath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackpath/refs/heads/main/security/stackpath-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Edge Computing
- Content Delivery Network
- Web Application Firewall
- DNS
- Object Storage
- Serverless
- Defunct
---
