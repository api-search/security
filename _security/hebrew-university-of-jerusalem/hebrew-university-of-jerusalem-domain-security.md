---
description: ''
domains:
- caa:
  - 0 issuewild "harica.gr"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: huji.ac.il
  spf: true
hosts:
- cert_expires: Dec  9 14:47:50 2026 GMT
  host: en.huji.ac.il
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 12:59:18 2026 GMT
  host: en.libraries.huji.ac.il
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 14:47:50 2026 GMT
  host: scholars.huji.ac.il
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hebrew University Of Jerusalem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hebrew University of Jerusalem, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hebrew University of Jerusalem
provider_slug: hebrew-university-of-jerusalem
slug: hebrew-university-of-jerusalem-domain-security
source_filename: hebrew-university-of-jerusalem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.huji.ac.il\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 14:47:50 2026 GMT\n  hsts: false\n- host: en.libraries.huji.ac.il\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 12:59:18 2026 GMT\n  hsts: false\n- host: scholars.huji.ac.il\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 14:47:50 2026 GMT\n  hsts: false\ndomains:\n- domain: huji.ac.il\n  dnssec: false\n  caa:\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hebrew-university-of-jerusalem/refs/heads/main/security/hebrew-university-of-jerusalem-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Israel
---
