---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: billhop.com
  spf: true
hosts:
- cert_expires: Nov 22 17:12:15 2026 GMT
  host: billhop.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Billhop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billhop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Billhop
provider_slug: billhop
slug: billhop-domain-security
source_filename: billhop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billhop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 17:12:15 2026 GMT\n  hsts: false\ndomains:\n- domain: billhop.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billhop/refs/heads/main/security/billhop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- FinTech
- Payments
- Working Capital
- Supplier Management
- Corporate Cards
---
