---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: indianpincode.com
  spf: true
hosts:
- cert_expires: Sep 28 04:49:15 2026 GMT
  host: indianpincode.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indian Pincode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indian Pincode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Indian Pincode
provider_slug: indian-pincode
slug: indian-pincode-domain-security
source_filename: indian-pincode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indianpincode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:49:15 2026 GMT\n  hsts: null\ndomains:\n- domain: indianpincode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indian-pincode/refs/heads/main/security/indian-pincode-domain-security.yml
summary_line: TLSv1.3
tags:
- Government
- Public APIs
---
