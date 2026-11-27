---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prevounce.com
  spf: true
hosts:
- cert_expires: Jan 17 07:31:16 2027 GMT
  host: prevounce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prevounce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prevounce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prevounce
provider_slug: prevounce
slug: prevounce-domain-security
source_filename: prevounce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prevounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 07:31:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prevounce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/prevounce/security/prevounce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Remote Monitoring
- Artificial Intelligence
- Software-as-a-Service
- Telehealth
---
