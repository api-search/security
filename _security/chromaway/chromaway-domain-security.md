---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chromaway.com
  spf: true
hosts:
- cert_expires: Dec 27 18:58:39 2026 GMT
  host: chromaway.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chromaway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChromaWay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ChromaWay
provider_slug: chromaway
slug: chromaway-domain-security
source_filename: chromaway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chromaway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 18:58:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: chromaway.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chromaway/refs/heads/main/security/chromaway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Web3
- Platform
- Consulting
- Ventures
- Artificial Intelligence
---
