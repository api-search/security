---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: verisign.com
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.verisign.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: developer.verisign.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.verisign.com
  https: false
kind: domain-security
layout: security
method: probed
name: Verisign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VeriSign, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: VeriSign
provider_slug: verisign
slug: verisign-domain-security
source_filename: verisign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verisign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.verisign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\n- host: api.verisign.com\n  https: false\ndomains:\n- domain: verisign.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verisign/refs/heads/main/security/verisign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DNS
- Internet Infrastructure
- Security
---
