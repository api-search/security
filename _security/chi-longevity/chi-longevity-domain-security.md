---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: chilongevity.com
  spf: true
hosts:
- cert_expires: Aug 25 23:07:33 2026 GMT
  host: chilongevity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chi Longevity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chi Longevity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Chi Longevity
provider_slug: chi-longevity
slug: chi-longevity-domain-security
source_filename: chi-longevity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chilongevity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:07:33 2026 GMT\n  hsts: false\ndomains:\n- domain: chilongevity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chi-longevity/refs/heads/main/security/chi-longevity-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Longevity
- Healthcare
- Healthy Aging
- Precision Health
- Wellness
- Singapore
---
