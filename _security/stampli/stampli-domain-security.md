---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog;cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stampli.com
  spf: true
hosts:
- cert_expires: Oct  8 18:30:59 2026 GMT
  host: www.stampli.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stampli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stampli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stampli
provider_slug: stampli
slug: stampli-domain-security
source_filename: stampli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stampli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:30:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: stampli.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog;cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stampli/refs/heads/main/security/stampli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounts Payable
- AP Automation
- Procure-to-Pay
- Invoice Management
- Vendor Management
- ERP Integration
- FinTech
- No Public API
- Gated API
---
