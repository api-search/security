---
description: ''
domains:
- caa:
  - 0 iodef "mailto:mimteam@usbank.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:domainadmin@usbank.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bentoforbusiness.com
  spf: true
hosts:
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: bentoforbusiness.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bento Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bento, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bento
provider_slug: bento
slug: bento-domain-security
source_filename: bento-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bentoforbusiness.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bentoforbusiness.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:mimteam@usbank.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:domainadmin@usbank.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bento/refs/heads/main/security/bento-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Fintech
- Payments
- Spend Management
- Expense Management
- Corporate Cards
- Virtual Cards
- Small Business
- Acquired
---
