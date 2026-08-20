---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ssfcu.org
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: ssfcu.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Security Service Fcu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Security Service Federal Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Security Service Federal Credit Union
provider_slug: security-service-fcu
slug: security-service-fcu-domain-security
source_filename: security-service-fcu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ssfcu.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ssfcu.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/security-service-fcu/refs/heads/main/security/security-service-fcu-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Credit Union
- Open Finance
- Data Aggregation
---
