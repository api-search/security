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
  domain: bmsstudyconnect.com
  spf: false
hosts:
- cert_expires: Sep  3 09:56:23 2026 GMT
  host: www.bms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 09:56:23 2026 GMT
  host: www.bmsstudyconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bristol Myers Squibb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bristol Myers Squibb, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bristol Myers Squibb
provider_slug: bristol-myers-squibb
slug: bristol-myers-squibb-domain-security
source_filename: bristol-myers-squibb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:56:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bmsstudyconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:56:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bmsstudyconnect.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bristol-myers-squibb/refs/heads/main/security/bristol-myers-squibb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pharmaceutical
- Biopharmaceutical
- Oncology
- Immunology
- Cardiovascular
- Clinical Trials
- Digital Health
- Fortune 500
---
