---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aidaly.com
  spf: true
hosts:
- cert_expires: Dec  1 17:56:53 2026 GMT
  host: www.aidaly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aidaly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aidaly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aidaly
provider_slug: aidaly
slug: aidaly-domain-security
source_filename: aidaly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aidaly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 17:56:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aidaly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidaly/refs/heads/main/security/aidaly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Home Care
- Caregiving
- Medicaid
- Health Tech
- Digital Health
- Benefits
- Workforce
- United States
- Company
---
