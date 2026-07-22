---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 410labs.com
  spf: true
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: 410labs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 410 Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 410 Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 410 Labs
provider_slug: 410-labs
slug: 410-labs-domain-security
source_filename: 410-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 410labs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 410labs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/410-labs/refs/heads/main/security/410-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email
- Productivity
- Inbox Management
- Email Cleanup
- Consumer Software
- Startup
---
