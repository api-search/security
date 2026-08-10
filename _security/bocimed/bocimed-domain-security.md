---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bocimed.com
  mx:
  - 5 mxbiz1.qq.com.
  - 10 mxbiz2.qq.com.
  nameservers:
  - dns21.hichina.com.
  - dns22.hichina.com.
  spf: true
  spf_record: v=spf1 include:spf.mail.qq.com ~all
hosts:
- host: www.bocimed.com
  hsts: null
  http: 200
  https: false
  https_port_open: true
  server: wts/1.7.4
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
- host: en.bocimed.com
  hsts: null
  http: 200
  https: false
  https_port_open: true
  server: wts/1.7.4
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
- host: bocimed.com
  hsts: null
  http: null
  https: false
  https_port_open: false
  tls_cert_error: timed out
kind: domain-security
layout: security
method: probed
name: Bocimed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BociMed, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BociMed
provider_slug: bocimed
slug: bocimed-domain-security
source_filename: bocimed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts\nnotes: >-\n  Every BociMed web host answers on port 443 but presents a self-signed certificate,\n  so no host completes a trusted TLS handshake. The public site is served over plain\n  HTTP only (http://www.bocimed.com/, http://en.bocimed.com/), with no HSTS. The apex\n  bocimed.com does not answer HTTP or HTTPS at all — only www and en resolve to a\n  serving origin. Absence of a record below is observed data, not a gap in the probe.\nhosts:\n- host: www.bocimed.com\n  https: false\n  https_port_open: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed\n    certificate (_ssl.c:1082)'\n  http: 200\n  hsts: null\n  server: wts/1.7.4\n- host: en.bocimed.com\n  https: false\n  https_port_open: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed\n    certificate (_ssl.c:1082)'\n  http: 200\n  hsts:\
  \ null\n  server: wts/1.7.4\n- host: bocimed.com\n  https: false\n  https_port_open: false\n  tls_cert_error: timed out\n  http: null\n  hsts: null\ndomains:\n- domain: bocimed.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.mail.qq.com ~all\n  dmarc: false\n  mx:\n  - 5 mxbiz1.qq.com.\n  - 10 mxbiz2.qq.com.\n  nameservers:\n  - dns21.hichina.com.\n  - dns22.hichina.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bocimed/refs/heads/main/security/bocimed-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Pharmaceuticals
- Life Sciences
- Contract Research Organization
- CDMO
- Drug Delivery
- Clinical Research
- Manufacturing
- China
- Shanghai
---
