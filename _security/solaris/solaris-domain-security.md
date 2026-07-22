---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solarisgroup.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solarisbank.de
  spf: true
hosts:
- cert_expires: Sep  8 10:05:00 2026 GMT
  host: www.solarisgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 22:19:51 2026 GMT
  host: docs.solarisgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: api.solarisbank.de
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solaris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solaris, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Solaris
provider_slug: solaris
slug: solaris-domain-security
source_filename: solaris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solarisgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 10:05:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.solarisgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:19:51 2026 GMT\n  hsts: false\n- host: api.solarisbank.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: solarisgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: solarisbank.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solaris/refs/heads/main/security/solaris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Banking
- Banking as a Service
- Embedded Finance
- Payments
- SEPA
- Cards
- KYC
- Lending
- Compliance
- OAuth2
- Webhooks
- Germany
---
