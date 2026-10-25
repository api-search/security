---
api_specs:
- filename: nthu-data-api.yaml
  format: yaml
  label: NTHU Data API
  slug: nthu-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/_original/nthu-data-api.yaml
- filename: nthu-oauth-api-openapi.yml
  format: yaml
  label: National Tsing Hua University O Auth API
  slug: nthu-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-oauth-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nthu.edu.tw
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nthusa.tw
  spf: true
hosts:
- cert_expires: Apr 30 15:59:59 2027 GMT
  host: www.nthu.edu.tw
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 12 15:59:59 2026 GMT
  host: nthu-en.site.nthu.edu.tw
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  9 12:41:44 2026 GMT
  host: api.nthusa.tw
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Nthu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Tsing Hua University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: National Tsing Hua University
provider_slug: nthu
slug: nthu-domain-security
source_filename: nthu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nthu.edu.tw\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 30 15:59:59 2027 GMT\n  hsts: false\n- host: nthu-en.site.nthu.edu.tw\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 15:59:59 2026 GMT\n  hsts: null\n- host: api.nthusa.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 12:41:44 2026 GMT\n  hsts: null\ndomains:\n- domain: nthu.edu.tw\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nthusa.tw\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/security/nthu-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Taiwan
- Public Research University
- Identity
- Authentication
- Open Data
- Campus
- Course Catalog
- Research Repository
- Library
- Identity Federation
---
