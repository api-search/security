---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: chattermill.com
  spf: true
hosts:
- cert_expires: Dec 13 10:53:28 2026 GMT
  host: chattermill.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chattermill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chattermill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Chattermill
provider_slug: chattermill
slug: chattermill-domain-security
source_filename: chattermill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chattermill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 10:53:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chattermill.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chattermill/refs/heads/main/security/chattermill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Voice of Customer
- Feedback Analysis
- Enterprise
---
