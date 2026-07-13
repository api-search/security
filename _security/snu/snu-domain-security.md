---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: snu.ac.kr
  spf: true
hosts:
- cert_expires: Aug 10 02:17:02 2026 GMT
  host: en.snu.ac.kr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: s-space.snu.ac.kr
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Snu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seoul National University, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Seoul National University
provider_slug: snu
slug: snu-domain-security
source_filename: snu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.snu.ac.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 02:17:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: s-space.snu.ac.kr\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: snu.ac.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snu/refs/heads/main/security/snu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Institutional Repository
- OAI-PMH
- South Korea
---
