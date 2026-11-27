---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vish.com
  spf: true
hosts:
- cert_expires: Jan 10 04:54:16 2027 GMT
  host: vish.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vish
provider_slug: vish-com
slug: vish-com-domain-security
source_filename: vish-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vish.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 04:54:16 2027 GMT\n  hsts: false\ndomains:\n- domain: vish.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/vish-com/security/vish-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Health
- Wellness
- Portal
- Healthcare
- Company
---
