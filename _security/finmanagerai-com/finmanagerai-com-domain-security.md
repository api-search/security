---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: finmanagerai.com
  spf: true
hosts:
- cert_expires: Jan 26 22:46:42 2027 GMT
  host: finmanagerai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FinManager AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FinManager AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FinManager AI
provider_slug: finmanagerai-com
slug: finmanagerai-com-domain-security
source_filename: finmanagerai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finmanagerai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 22:46:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: finmanagerai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/finmanagerai-com/security/finmanagerai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Artificial Intelligence
- Investment
- Platform
- Fintech
---
