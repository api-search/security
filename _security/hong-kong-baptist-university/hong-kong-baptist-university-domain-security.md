---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hkbu.edu.hk
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.hkbu.edu.hk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: buidp01.hkbu.edu.hk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: genai.hkbu.edu.hk
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hong Kong Baptist University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hong Kong Baptist University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hong Kong Baptist University
provider_slug: hong-kong-baptist-university
slug: hong-kong-baptist-university-domain-security
source_filename: hong-kong-baptist-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hkbu.edu.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: buidp01.hkbu.edu.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\n- host: genai.hkbu.edu.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: hkbu.edu.hk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hong-kong-baptist-university/refs/heads/main/security/hong-kong-baptist-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- Hong Kong
- UGC-Funded
- Identity Federation
- Shibboleth
- SAML
- eduGAIN
- Learning Management
- LTI
- Artificial Intelligence
- Research Information
- Elsevier Pure
---
