---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wiredscore.com
  spf: true
hosts:
- cert_expires: Sep 14 14:00:04 2026 GMT
  host: wiredscore.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wiredscore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WiredScore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: WiredScore
provider_slug: wiredscore
slug: wiredscore-domain-security
source_filename: wiredscore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wiredscore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:00:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wiredscore.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wiredscore/refs/heads/main/security/wiredscore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Vertical Software
- Real Estate
- PropTech
- Building Certification
- Smart Buildings
- Digital Connectivity
- Sustainability
---
