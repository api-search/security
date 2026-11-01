---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: farmwiselabs.com
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: farmwiselabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Farmwiselabs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FarmWise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FarmWise
provider_slug: farmwiselabs-com
slug: farmwiselabs-com-domain-security
source_filename: farmwiselabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farmwiselabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: farmwiselabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/farmwiselabs-com/security/farmwiselabs-com-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- AgriTech
- Robotics
- Automation
- AI
---
