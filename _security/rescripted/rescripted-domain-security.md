---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rescripted.com
  spf: true
hosts:
- cert_expires: Aug 26 12:52:56 2026 GMT
  host: rescripted.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rescripted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rescripted, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rescripted
provider_slug: rescripted
slug: rescripted-domain-security
source_filename: rescripted-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rescripted.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 12:52:56 2026 GMT\n  hsts: false\ndomains:\n- domain: rescripted.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rescripted/refs/heads/main/security/rescripted-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Women's Health
- Digital Health
- Femtech
- Fertility
- Artificial Intelligence
- Consumer Health
- Wellness
---
