---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: d2g-insite.com
  spf: false
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: www.d2g-insite.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: D2G Oncology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D2G Oncology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: D2G Oncology
provider_slug: d2g-oncology
slug: d2g-oncology-domain-security
source_filename: d2g-oncology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.d2g-insite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: d2g-insite.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d2g-oncology/refs/heads/main/security/d2g-oncology-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Oncology
- Healthcare
- Biotechnology
- Therapeutics
- Life Sciences
- Precision Medicine
- Functional Genomics
---
