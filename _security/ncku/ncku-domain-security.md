---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ncku.edu.tw
  spf: true
hosts:
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: web.ncku.edu.tw
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: data.ncku.edu.tw
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Missing Subject Key Identifier (_ssl.c:1082)'
- host: www.lib.ncku.edu.tw
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Missing Subject Key Identifier (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Ncku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Cheng Kung University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: National Cheng Kung University
provider_slug: ncku
slug: ncku-domain-security
source_filename: ncku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: web.ncku.edu.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: null\n- host: data.ncku.edu.tw\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Missing Subject\n    Key Identifier (_ssl.c:1082)'\n  hsts: null\n- host: www.lib.ncku.edu.tw\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Missing Subject\n    Key Identifier (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ncku.edu.tw\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ncku/refs/heads/main/security/ncku-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Library
- Taiwan
---
