---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chinaisti.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.chinaisti.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chinaist Testing Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChinaiST Testing Service, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ChinaiST Testing Service
provider_slug: chinaist-testing-service
slug: chinaist-testing-service-domain-security
source_filename: chinaist-testing-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chinaisti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chinaisti.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chinaist-testing-service/refs/heads/main/security/chinaist-testing-service-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- HighTech
- Testing
- Reliability
- Semiconductors
---
