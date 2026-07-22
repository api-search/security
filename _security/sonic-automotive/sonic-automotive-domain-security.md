---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sonic-automotive.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: echopark.com
  spf: true
hosts:
- host: www.sonic-automotive.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.echopark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonic Automotive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonic Automotive, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sonic Automotive
provider_slug: sonic-automotive
slug: sonic-automotive-domain-security
source_filename: sonic-automotive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sonic-automotive.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: www.echopark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sonic-automotive.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: echopark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonic-automotive/refs/heads/main/security/sonic-automotive-domain-security.yml
summary_line: TLSv1.3
tags:
- Automotive
- Retail
- Dealership
- Used Vehicles
- Digital Retail
- Fortune 500
---
