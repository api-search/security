---
description: ''
domains:
- caa:
  - 0 contactemail "sbbgrp-ssp-pmp@g.softbank.co.jp"
  - 0 contactemail "SBBGRP-SPO2-IAA@g.softbank.co.jp"
  dmarc: false
  dnssec: false
  domain: softbank.jp
  spf: true
hosts:
- cert_expires: Jan 28 14:59:00 2027 GMT
  host: www.softbank.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Softbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoftBank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SoftBank
provider_slug: softbank
slug: softbank-domain-security
source_filename: softbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.softbank.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 14:59:00 2027 GMT\n  hsts: false\ndomains:\n- domain: softbank.jp\n  dnssec: false\n  caa:\n  - 0 contactemail \"sbbgrp-ssp-pmp@g.softbank.co.jp\"\n  - 0 contactemail \"SBBGRP-SPO2-IAA@g.softbank.co.jp\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/softbank/refs/heads/main/security/softbank-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Telecommunications
- Technology
- Investment
- Artificial Intelligence
- Robotics
---
