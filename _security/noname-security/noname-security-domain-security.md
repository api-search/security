---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nonamesecurity.com
  spf: true
hosts:
- cert_expires: Sep  7 13:00:08 2026 GMT
  host: nonamesecurity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noname Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noname Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Noname Security
provider_slug: noname-security
slug: noname-security-domain-security
source_filename: noname-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nonamesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 13:00:08 2026 GMT\n  hsts: null\ndomains:\n- domain: nonamesecurity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noname-security/refs/heads/main/security/noname-security-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- API Discovery
- API Security
- API Testing
- Posture Management
- Runtime Protection
- Shadow APIs
---
