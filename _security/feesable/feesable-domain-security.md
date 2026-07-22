---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: feesable.ai
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: feesable.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Feesable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feesable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Feesable
provider_slug: feesable
slug: feesable-domain-security
source_filename: feesable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: feesable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: feesable.ai\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feesable/refs/heads/main/security/feesable-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Embedded Finance
- Fintech
- Lending
- Loan Origination
- Debt Capital Management
- Treasury Management
- Credit Decisioning
- KYC
- Payments Infrastructure
---
