---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: noxtua.com
  spf: true
hosts:
- cert_expires: Sep  5 15:00:03 2026 GMT
  host: www.noxtua.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xayn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xayn (now Noxtua), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Xayn (now Noxtua)
provider_slug: xayn
slug: xayn-domain-security
source_filename: xayn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.noxtua.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:00:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: noxtua.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xayn/refs/heads/main/security/xayn-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Legal Tech
- Privacy
- Search
- Federated Learning
- Machine Learning
- Germany
---
