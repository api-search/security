---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 iodef "mailto:angel.torres@getmurphy.ai"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getmurphy.ai
  spf: true
hosts:
- cert_expires: Oct 16 21:31:53 2026 GMT
  host: www.getmurphy.ai
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Murphy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Murphy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Murphy
provider_slug: murphy
slug: murphy-domain-security
source_filename: murphy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getmurphy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 21:31:53 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\ndomains:\n- domain: getmurphy.ai\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:angel.torres@getmurphy.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/murphy/refs/heads/main/security/murphy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Artificial Intelligence
- Debt Collection
- Voice AI
- Financial Services
- Collections
---
