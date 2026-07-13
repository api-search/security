---
api_specs:
- filename: yonsei-pure.yaml
  format: yaml
  label: Yonsei Research Information Portal (Elsevier Pure)
  slug: pure
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yonsei/refs/heads/main/openapi/yonsei-pure.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yonsei.ac.kr
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: elsevierpure.com
  spf: false
hosts:
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: www.yonsei.ac.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 15:59:11 2026 GMT
  host: yonsei.elsevierpure.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: ir.ymlib.yonsei.ac.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yonsei Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yonsei University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yonsei University
provider_slug: yonsei
slug: yonsei-domain-security
source_filename: yonsei-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yonsei.ac.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\n- host: yonsei.elsevierpure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 15:59:11 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: ir.ymlib.yonsei.ac.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: yonsei.ac.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: elsevierpure.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yonsei/refs/heads/main/security/yonsei-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Repository
- South Korea
- Seoul
---
