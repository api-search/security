---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: augmentcode.com
  spf: true
hosts:
- cert_expires: Sep 14 18:17:44 2026 GMT
  host: www.augmentcode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 11:10:39 2026 GMT
  host: docs.augmentcode.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Augment Code Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augment Code, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Augment Code
provider_slug: augment-code
slug: augment-code-domain-security
source_filename: augment-code-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.augmentcode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:17:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.augmentcode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:10:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: augmentcode.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augment-code/refs/heads/main/security/augment-code-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Coding Agent
- Context Engine
- IDE Plugin
- Cosmos
- Auggie CLI
- Software Engineering
---
