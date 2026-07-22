---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:itmanager@provablelabs.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: provablemarkets.com
  spf: true
hosts:
- cert_expires: Sep 25 05:04:29 2026 GMT
  host: developer.provablemarkets.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 13:08:19 2026 GMT
  host: provablemarkets.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Provable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Provable, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Provable
provider_slug: provable
slug: provable-domain-security
source_filename: provable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.provablemarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:04:29 2026 GMT\n  hsts: false\n- host: provablemarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:08:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: provablemarkets.com\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:itmanager@provablelabs.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provable/refs/heads/main/security/provable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Securities Lending
- Capital Markets
- Fintech
- Trading
- Alternative Trading System
- Post-Trade
- gRPC
- FIX
---
