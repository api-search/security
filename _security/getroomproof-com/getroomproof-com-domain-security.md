---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: getroomproof.com
  spf: true
hosts:
- cert_expires: Dec 14 12:41:32 2026 GMT
  host: getroomproof.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Roomproof Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roomproof, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Roomproof
provider_slug: getroomproof-com
slug: getroomproof-com-domain-security
source_filename: getroomproof-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getroomproof.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 12:41:32 2026 GMT\n  hsts: false\ndomains:\n- domain: getroomproof.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/getroomproof-com/security/getroomproof-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
