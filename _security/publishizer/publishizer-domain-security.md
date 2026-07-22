---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: publishizer.com
  spf: true
hosts:
- cert_expires: Sep  3 21:03:57 2026 GMT
  host: publishizer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Publishizer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Publishizer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Publishizer
provider_slug: publishizer
slug: publishizer-domain-security
source_filename: publishizer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: publishizer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 21:03:57 2026 GMT\n  hsts: false\ndomains:\n- domain: publishizer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publishizer/refs/heads/main/security/publishizer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Publishing
- Crowdfunding
- Books
- Authors
- Literary Agency
- Marketplace
---
