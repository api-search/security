---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: withpage.com
  spf: true
hosts:
- cert_expires: Sep 23 05:38:44 2026 GMT
  host: www.withpage.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Page Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Page, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Page
provider_slug: page
slug: page-domain-security
source_filename: page-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withpage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:38:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: withpage.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/page/refs/heads/main/security/page-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government Relations
- Legislative Intelligence
- Regulatory Affairs
- Policy
- GovTech
- Artificial Intelligence
- Compliance
- SaaS
---
