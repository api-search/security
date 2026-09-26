---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: anique.jp
  spf: true
hosts:
- cert_expires: Dec 12 09:01:03 2026 GMT
  host: anique.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anique Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anique, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Anique
provider_slug: anique
slug: anique-domain-security
source_filename: anique-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anique.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 09:01:03 2026 GMT\n  hsts: false\ndomains:\n- domain: anique.jp\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anique/refs/heads/main/security/anique-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- IP
- Digital
- Merchandise
- Japan
---
