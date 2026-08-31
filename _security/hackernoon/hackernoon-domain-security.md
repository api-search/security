---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hackernoon.com
  spf: true
hosts:
- cert_expires: Nov  9 17:29:06 2026 GMT
  host: hackernoon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hackernoon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hackernoon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hackernoon
provider_slug: hackernoon
slug: hackernoon-domain-security
source_filename: hackernoon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hackernoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 17:29:06 2026 GMT\n  hsts: false\ndomains:\n- domain: hackernoon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hackernoon/refs/heads/main/security/hackernoon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Media
- Publishing
- Content
- Technology
- Developer Community
- AI Licensing
- Open-Source
- Syndication
- Content Licensing
---
