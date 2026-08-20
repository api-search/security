---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: accessfintech.com
  spf: true
hosts:
- cert_expires: Sep 12 03:58:59 2026 GMT
  host: www.accessfintech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 03:58:59 2026 GMT
  host: api.accessfintech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accessfintech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AccessFintech, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AccessFintech
provider_slug: accessfintech
slug: accessfintech-domain-security
source_filename: accessfintech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accessfintech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:58:59 2026 GMT\n  hsts: false\n- host: api.accessfintech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:58:59 2026 GMT\n  hsts: null\ndomains:\n- domain: accessfintech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accessfintech/refs/heads/main/security/accessfintech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial-Services
- Capital Markets
- Post-Trade
- Settlement
- Data Networks
- Reconciliation
- Fintech
- GraphQL
---
