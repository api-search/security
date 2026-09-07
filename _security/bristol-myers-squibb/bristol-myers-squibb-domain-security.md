---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bms.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bmsmedinfo.com
  spf: false
hosts:
- cert_expires: Nov 16 12:30:05 2026 GMT
  host: www.bms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 06:33:31 2026 GMT
  host: www.bmsmedinfo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 12:30:05 2026 GMT
  host: www.bmsclinicaltrials.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Bristol Myers Squibb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bristol Myers Squibb, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bristol Myers Squibb
provider_slug: bristol-myers-squibb
slug: bristol-myers-squibb-domain-security
source_filename: bristol-myers-squibb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 12:30:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bmsmedinfo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:33:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bmsclinicaltrials.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 12:30:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bmsmedinfo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bristol-myers-squibb/refs/heads/main/security/bristol-myers-squibb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pharmaceuticals
- Biopharmaceutical
- Oncology
- Immunology
- Cardiovascular
- Clinical Trials
- Digital Health
- Fortune 500
---
