---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: key.ai
  spf: true
hosts:
- cert_expires: Sep  5 13:59:05 2026 GMT
  host: key.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Key Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Key, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Key
provider_slug: key
slug: key-domain-security
source_filename: key-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: key.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:59:05 2026 GMT\n  hsts: null\ndomains:\n- domain: key.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/key/refs/heads/main/security/key-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Professional Networking
- Artificial Intelligence
- Community
- Introductions
- Networking
- B2B SaaS
---
