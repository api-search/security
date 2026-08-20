---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: liveoak.bank
  spf: true
hosts:
- cert_expires: Sep 20 16:40:13 2026 GMT
  host: www.liveoak.bank
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Live Oak Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Live Oak Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Live Oak Bank
provider_slug: live-oak-bank
slug: live-oak-bank-domain-security
source_filename: live-oak-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liveoak.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:40:13 2026 GMT\n  hsts: false\ndomains:\n- domain: liveoak.bank\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/live-oak-bank/refs/heads/main/security/live-oak-bank-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Small Business Lending
- SBA
- Embedded Banking
- Banking as a Service
- Digital Bank
- Open Finance
---
