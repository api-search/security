---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wrapbook.com
  spf: true
hosts:
- cert_expires: Sep 12 02:08:43 2026 GMT
  host: www.wrapbook.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wrapbook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wrapbook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wrapbook
provider_slug: wrapbook
slug: wrapbook-domain-security
source_filename: wrapbook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wrapbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:08:43 2026 GMT\n  hsts: false\ndomains:\n- domain: wrapbook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wrapbook/refs/heads/main/security/wrapbook-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Entertainment
- Payroll
- Production Accounting
- Accounts Payable
- Film
- Television
- Fintech
---
