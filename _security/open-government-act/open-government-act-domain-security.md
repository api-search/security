---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: act.gov.au
  spf: true
hosts:
- cert_expires: Nov  1 19:08:08 2026 GMT
  host: www.data.act.gov.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Open Government Act Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, ACT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Open Government, ACT
provider_slug: open-government-act
slug: open-government-act-domain-security
source_filename: open-government-act-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.data.act.gov.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  1 19:08:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: act.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-act/refs/heads/main/security/open-government-act-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
