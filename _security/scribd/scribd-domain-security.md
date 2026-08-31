---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scribd.com
  spf: true
hosts:
- cert_expires: Sep 25 17:48:10 2026 GMT
  host: www.scribd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scribd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scribd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scribd
provider_slug: scribd
slug: scribd-domain-security
source_filename: scribd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scribd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:48:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: scribd.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scribd/refs/heads/main/security/scribd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Documents
- eBooks
- Audiobooks
- Publishing
- Content
- Subscription
- Media
- Reading
---
