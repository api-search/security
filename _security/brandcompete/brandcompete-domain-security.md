---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brandcompete.com
  spf: true
hosts:
- cert_expires: Jan 10 14:08:32 2027 GMT
  host: brandcompete.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brandcompete Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandcompete, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Brandcompete
provider_slug: brandcompete
slug: brandcompete-domain-security
source_filename: brandcompete-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brandcompete.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 14:08:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brandcompete.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandcompete/refs/heads/main/security/brandcompete-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Cloud Consulting
- Data Intelligence
- Process Automation
- Enterprise Software
- Artificial Intelligence
- GDPR Compliance
---
