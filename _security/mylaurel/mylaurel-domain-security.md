---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mylaurelhealth.com
  spf: true
hosts:
- cert_expires: Oct 15 18:57:03 2026 GMT
  host: www.mylaurelhealth.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mylaurel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for myLaurel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: myLaurel
provider_slug: mylaurel
slug: mylaurel-domain-security
source_filename: mylaurel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mylaurelhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:57:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mylaurelhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mylaurel/refs/heads/main/security/mylaurel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Healthcare
- Home Health
- Acute Care
- Transitional Care
- Digital Health
- Value-Based Care
---
