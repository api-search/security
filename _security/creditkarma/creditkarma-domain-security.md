---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:domains-caa@creditkarma.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: creditkarma.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: creditkarma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Creditkarma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CreditKarma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CreditKarma
provider_slug: creditkarma
slug: creditkarma-domain-security
source_filename: creditkarma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creditkarma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: creditkarma.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:domains-caa@creditkarma.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creditkarma/refs/heads/main/security/creditkarma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Personal Finance
- Fintech
- Credit Scores
- Credit Monitoring
- Financial Services
- Consumer Finance
---
