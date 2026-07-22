---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@flexfinance.ai"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flexfinance.ai
  spf: true
hosts:
- cert_expires: Sep 30 16:01:01 2026 GMT
  host: flexfinance.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flex
provider_slug: flex
slug: flex-domain-security
source_filename: flex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flexfinance.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:01:01 2026 GMT\n  hsts: false\ndomains:\n- domain: flexfinance.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@flexfinance.ai\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flex/refs/heads/main/security/flex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- FinTech
- Financial Services
- Payments
- Rent Payments
- Consumer Finance
- Bill Pay
- Real Estate
---
