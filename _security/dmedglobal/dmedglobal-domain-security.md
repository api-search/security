---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dmedglobal.com
  spf: true
hosts:
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: dmedglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dmedglobal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dMed Global (Caidya), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: dMed Global (Caidya)
provider_slug: dmedglobal
slug: dmedglobal-domain-security
source_filename: dmedglobal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dmedglobal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dmedglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dmedglobal/refs/heads/main/security/dmedglobal-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Clinical Research
- Contract Research Organization
- Healthcare
- Life Sciences
- Pharmaceutical
- Clinical Trials
---
