---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: vic.gov.au
  spf: true
hosts:
- cert_expires: Aug 19 16:39:26 2026 GMT
  host: www.data.vic.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Victoria State Government Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Victoria State Government, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Open Government, Victoria State Government
provider_slug: open-government-victoria-state-government
slug: open-government-victoria-state-government-domain-security
source_filename: open-government-victoria-state-government-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.data.vic.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 16:39:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vic.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-victoria-state-government/refs/heads/main/security/open-government-victoria-state-government-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
