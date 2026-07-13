---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: goguardian.com
  spf: true
hosts:
- cert_expires: Oct  2 19:12:51 2026 GMT
  host: www.goguardian.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: support.goguardian.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: based.goguardian.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goguardian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoGuardian, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: GoGuardian
provider_slug: goguardian
slug: goguardian-domain-security
source_filename: goguardian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goguardian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:12:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.goguardian.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: based.goguardian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: goguardian.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goguardian/refs/heads/main/security/goguardian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- EdTech
- K-12
- Content Filtering
- Classroom Management
- Student Safety
- Rostering
- OneRoster
- Partner API
---
