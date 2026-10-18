---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: justgptit.com
  spf: false
hosts:
- cert_expires: Dec  5 14:05:27 2026 GMT
  host: justgptit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Justgptit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Just Gpt It, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Just Gpt It
provider_slug: justgptit
slug: justgptit-domain-security
source_filename: justgptit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justgptit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 14:05:27 2026 GMT\n  hsts: false\ndomains:\n- domain: justgptit.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justgptit/refs/heads/main/security/justgptit-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- Text-Generation
- API
- GPT
---
