---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bjgoodwill.com
  spf: true
hosts:
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: www.bjgoodwill.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bjgoodwill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beijing Goodwill (bjgoodwill), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Beijing Goodwill (bjgoodwill)
provider_slug: bjgoodwill
slug: bjgoodwill-domain-security
source_filename: bjgoodwill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bjgoodwill.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bjgoodwill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bjgoodwill/refs/heads/main/security/bjgoodwill-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Healthcare
- Health IT
- Electronic Medical Records
- EMR
- Hospital Information Systems
- Medical Big Data
- China
---
