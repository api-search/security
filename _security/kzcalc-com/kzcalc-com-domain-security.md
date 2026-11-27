---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: kzcalc.com
  spf: false
hosts:
- cert_expires: Dec 31 11:56:27 2026 GMT
  host: kzcalc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KzCalc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KzCalc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: KzCalc
provider_slug: kzcalc-com
slug: kzcalc-com-domain-security
source_filename: kzcalc-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kzcalc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 11:56:27 2026 GMT\n  hsts: false\ndomains:\n- domain: kzcalc.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kzcalc-com/security/kzcalc-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Calculator
- Kazakhstan
- Finance
- Education
- Government
---
