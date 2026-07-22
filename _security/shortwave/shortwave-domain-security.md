---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: shortwave.com
  spf: true
hosts:
- cert_expires: Oct 11 15:17:52 2026 GMT
  host: www.shortwave.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shortwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shortwave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Shortwave
provider_slug: shortwave
slug: shortwave-domain-security
source_filename: shortwave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shortwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 15:17:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shortwave.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shortwave/refs/heads/main/security/shortwave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email
- Email Client
- Artificial Intelligence
- AI Assistant
- Productivity
- Model Context Protocol
- Gmail
- Google Workspace
- Collaboration
---
