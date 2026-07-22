---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oshihealth.com
  spf: true
hosts:
- cert_expires: Sep 25 04:30:50 2026 GMT
  host: oshihealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oshi Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oshi Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oshi Health
provider_slug: oshi-health
slug: oshi-health-domain-security
source_filename: oshi-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oshihealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 04:30:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oshihealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oshi-health/refs/heads/main/security/oshi-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Telehealth
- Gastroenterology
- Digital Health
- Virtual Care
---
