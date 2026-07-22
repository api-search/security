---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adelphic.com
  spf: true
hosts:
- cert_expires: Oct  7 17:26:25 2026 GMT
  host: www.adelphic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adelphic Mobile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adelphic Mobile *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adelphic Mobile *
provider_slug: adelphic-mobile
slug: adelphic-mobile-domain-security
source_filename: adelphic-mobile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adelphic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:26:25 2026 GMT\n  hsts: false\ndomains:\n- domain: adelphic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adelphic-mobile/refs/heads/main/security/adelphic-mobile-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Advertising
- AdTech
- Programmatic Advertising
- Demand Side Platform
- DSP
- Marketing
- Connected TV
---
