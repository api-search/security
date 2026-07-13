---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hanyang.ac.kr
  spf: true
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: www.hanyang.ac.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.hanyang.ac.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hanyang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hanyang University, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hanyang University
provider_slug: hanyang
slug: hanyang-domain-security
source_filename: hanyang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hanyang.ac.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.hanyang.ac.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hanyang.ac.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanyang/refs/heads/main/security/hanyang-domain-security.yml
summary_line: TLSv1.2
tags:
- Education
- Higher Education
- University
- South Korea
- Seoul
- Open API
- OAuth
---
