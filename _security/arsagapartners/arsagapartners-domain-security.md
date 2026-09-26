---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arsaga.jp
  spf: true
hosts:
- cert_expires: Nov 13 10:33:47 2026 GMT
  host: www.arsaga.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arsagapartners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arsagapartners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arsagapartners
provider_slug: arsagapartners
slug: arsagapartners-domain-security
source_filename: arsagapartners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arsaga.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 10:33:47 2026 GMT\n  hsts: false\ndomains:\n- domain: arsaga.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arsagapartners/refs/heads/main/security/arsagapartners-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consulting
- AI
- Software Development
- Japan
---
