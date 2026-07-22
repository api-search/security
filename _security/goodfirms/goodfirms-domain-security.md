---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: goodfirms.co
  spf: true
hosts:
- cert_expires: Oct  6 06:58:01 2026 GMT
  host: www.goodfirms.co
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goodfirms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoodFirms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: GoodFirms
provider_slug: goodfirms
slug: goodfirms-domain-security
source_filename: goodfirms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodfirms.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:58:01 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: goodfirms.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodfirms/refs/heads/main/security/goodfirms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- B2B
- IT Services
- Software Reviews
---
