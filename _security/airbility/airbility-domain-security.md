---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: airbility.co.kr
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: airbility.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Airbility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airbility, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Airbility
provider_slug: airbility
slug: airbility-domain-security
source_filename: airbility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airbility.co.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: airbility.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbility/refs/heads/main/security/airbility-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
