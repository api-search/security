---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: betteryou.com
  spf: true
hosts:
- cert_expires: Oct 30 19:48:35 2026 GMT
  host: betteryou.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Betteryou Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetterYou, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BetterYou
provider_slug: betteryou
slug: betteryou-domain-security
source_filename: betteryou-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betteryou.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 19:48:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: betteryou.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betteryou/refs/heads/main/security/betteryou-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Nutrition
- Supplements
- Health
- Wellness
---
