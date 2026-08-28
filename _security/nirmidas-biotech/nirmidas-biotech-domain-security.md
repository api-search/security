---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nirmidas.com
  spf: true
hosts:
- host: www.nirmidas.com
  hsts: null
  http_to_https_redirect: 301
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
  tls_certificate:
    days_expired_at_probe: 67
    expired: true
    issuer: C=CN, O=WoTrus CA Limited, CN=WoTrus DV Server CA
    not_after: '2026-06-20'
    not_before: '2025-05-20'
    subject: CN=www.nirmidas.com
kind: domain-security
layout: security
method: probed
name: Nirmidas Biotech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nirmidas Biotech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nirmidas Biotech
provider_slug: nirmidas-biotech
slug: nirmidas-biotech-domain-security
source_filename: nirmidas-biotech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nirmidas.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n  tls_certificate:\n    subject: CN=www.nirmidas.com\n    issuer: 'C=CN, O=WoTrus CA Limited, CN=WoTrus DV Server CA'\n    not_before: '2025-05-20'\n    not_after: '2026-06-20'\n    expired: true\n    days_expired_at_probe: 67\n  http_to_https_redirect: 301\ndomains:\n- domain: nirmidas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\nnotes: >-\n  MATERIAL FINDING — the public website of Nirmidas Biotech cannot be reached by a standards-compliant\n  HTTPS client. The leaf certificate served on www.nirmidas.com and nirmidas.com expired on 2026-06-20\n  and was still being served on 2026-08-26, so every browser and every automated client presents or\n  raises a certificate error\
  \ before any content is delivered. Every probe recorded in this repository\n  therefore had to disable certificate verification. Compounding it, the issuing CA is WoTrus CA Limited\n  (the successor of WoSign), whose roots are distrusted by the major browser trust stores — so even a\n  freshly reissued certificate from the same chain would not validate. The hosting is Alibaba/Wanwang\n  (www.nirmidas.com resolves via wh-au3su8zmnldkkubdddb.my3w.com to 198.11.174.219). No HSTS header is\n  served, DNSSEC is not enabled, no CAA records are published, and there is no DMARC record; an SPF\n  record is present.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nirmidas-biotech/refs/heads/main/security/nirmidas-biotech-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- Diagnostics
- Life Sciences
- Medical Imaging
- In Vitro Diagnostics
- Laboratory Instruments
- Research Reagents
- Nanotechnology
---
