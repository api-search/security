---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: intergiro.com
  spf: true
hosts:
- cert_expires: Jan 16 10:50:51 2027 GMT
  host: intergiro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intergiro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intergiro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Intergiro
provider_slug: intergiro
slug: intergiro-domain-security
source_filename: intergiro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intergiro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 10:50:51 2027 GMT\n  hsts: false\ndomains:\n- domain: intergiro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/intergiro/security/intergiro-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Banking
- Payments
- Fintech
- B2B
---
