---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: plooto.com
  spf: true
hosts:
- cert_expires: Sep 19 14:53:40 2026 GMT
  host: www.plooto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plooto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plooto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Plooto
provider_slug: plooto
slug: plooto-domain-security
source_filename: plooto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plooto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 14:53:40 2026 GMT\n  hsts: null\ndomains:\n- domain: plooto.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plooto/refs/heads/main/security/plooto-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Payments
- Canada
- Accounts Payable
- Accounts Receivable
- AP Automation
- AR Automation
- Bill Pay
- Money Transfer
- EFT
- ACH
- Cross-Border
- SMB
---
