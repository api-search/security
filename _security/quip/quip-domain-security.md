---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quip.com
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: quip.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: platform.quip.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quip, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quip
provider_slug: quip
slug: quip-domain-security
source_filename: quip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\n- host: platform.quip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: quip.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quip/refs/heads/main/security/quip-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Collaboration
- Productivity
- Documents
- Spreadsheets
- Team Chat
- Salesforce
---
