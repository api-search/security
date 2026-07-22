---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: seekout.io
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: app.seekout.io
  hsts: true
  hsts_max_age: 31535999
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seekout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SeekOut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SeekOut
provider_slug: seekout
slug: seekout-domain-security
source_filename: seekout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.seekout.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31535999\ndomains:\n- domain: seekout.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seekout/refs/heads/main/security/seekout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Recruiting
- Talent Acquisition
- HR Tech
- Sourcing
- Artificial Intelligence
- Candidate Search
- MCP
- Recruiting Automation
---
