---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: muckrack.com
  spf: true
hosts:
- cert_expires: Nov 13 23:31:06 2026 GMT
  host: muckrack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Muck Rack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Muck Rack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Muck Rack
provider_slug: muck-rack
slug: muck-rack-domain-security
source_filename: muck-rack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: muckrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:31:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: muckrack.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/muck-rack/refs/heads/main/security/muck-rack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Public Relations
- Media Monitoring
- Media Database
- Journalists
- Communications
- Press Releases
- Earned Media
- Social Listening
- Marketing
- News
- Analytics
- Company
---
