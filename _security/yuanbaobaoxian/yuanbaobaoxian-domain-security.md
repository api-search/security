---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: yuanbaobaoxian.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: yuanbaobaoxian.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yuanbaobaoxian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yuanbao (元保), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Yuanbao (元保)
provider_slug: yuanbaobaoxian
slug: yuanbaobaoxian-domain-security
source_filename: yuanbaobaoxian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yuanbaobaoxian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: yuanbaobaoxian.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuanbaobaoxian/refs/heads/main/security/yuanbaobaoxian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- Insurtech
- Online Insurance Distribution
- China
- Artificial Intelligence
- Financial Services
---
