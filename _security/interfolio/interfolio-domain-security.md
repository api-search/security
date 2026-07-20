---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: interfolio.com
  spf: true
hosts:
- cert_expires: Aug 23 13:17:59 2026 GMT
  host: www.interfolio.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Interfolio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interfolio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Interfolio
provider_slug: interfolio
slug: interfolio-domain-security
source_filename: interfolio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.interfolio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 13:17:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: interfolio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interfolio/refs/heads/main/security/interfolio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Higher Education
- Faculty Information System
- Faculty Activity Reporting
- Review Promotion Tenure
- Academic
- Research
---
