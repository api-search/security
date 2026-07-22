---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pandai.org
  spf: true
hosts:
- cert_expires: Oct  3 09:12:19 2026 GMT
  host: pandai.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pandai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pandai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pandai
provider_slug: pandai
slug: pandai-domain-security
source_filename: pandai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pandai.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:12:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pandai.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandai/refs/heads/main/security/pandai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Education
- EdTech
- E-Learning
- Online Learning
- Students
- Malaysia
- Assessment
---
