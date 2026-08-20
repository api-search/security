---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 1stdigital.com
  spf: true
hosts:
- cert_expires: Sep 30 20:48:19 2026 GMT
  host: 1stdigital.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: First Digital Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Digital Trust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: First Digital Trust
provider_slug: first-digital-trust
slug: first-digital-trust-domain-security
source_filename: first-digital-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1stdigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:48:19 2026 GMT\n  hsts: false\ndomains:\n- domain: 1stdigital.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-digital-trust/refs/heads/main/security/first-digital-trust-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Digital Assets
- Custody
- Trust Services
- Financial-Services
- Banking
- Payments
- Compliance
- Cryptocurrency
- Hong Kong
---
