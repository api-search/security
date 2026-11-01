---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fzu.edu.cn
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.fzu.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fuzhou University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fuzhou University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fuzhou University
provider_slug: fuzhou-university
slug: fuzhou-university-domain-security
source_filename: fuzhou-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fzu.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fzu.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fuzhou-university/security/fuzhou-university-domain-security.yml
summary_line: TLSv1.2
tags:
- University
- Education
- China
- Public
- Research
---
