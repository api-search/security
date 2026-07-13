---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: credibly.com
  spf: true
hosts:
- cert_expires: Sep 22 06:48:19 2026 GMT
  host: www.credibly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: api.credibly.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Credibly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credibly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Credibly
provider_slug: credibly
slug: credibly-domain-security
source_filename: credibly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.credibly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 06:48:19 2026 GMT\n  hsts: false\n- host: api.credibly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: credibly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credibly/refs/heads/main/security/credibly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Small Business Lending
- Merchant Cash Advance
- Working Capital
- Business Loans
- Fintech
- Lending API
- Partner Integration
---
