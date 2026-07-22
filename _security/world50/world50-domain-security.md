---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: world50.com
  spf: true
hosts:
- cert_expires: Aug 22 17:25:47 2026 GMT
  host: world50.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: World50 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World 50 Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: World 50 Group
provider_slug: world50
slug: world50-domain-security
source_filename: world50-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: world50.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 17:25:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: world50.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/world50/refs/heads/main/security/world50-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Executive Networking
- Peer Communities
- Leadership Development
- C-Suite
- Professional Services
- Membership
---
