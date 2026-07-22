---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dieboldnixdorf.com
  spf: true
hosts:
- cert_expires: Aug 14 23:59:59 2026 GMT
  host: www.dieboldnixdorf.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diebold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diebold Nixdorf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Diebold Nixdorf
provider_slug: diebold
slug: diebold-domain-security
source_filename: diebold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dieboldnixdorf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dieboldnixdorf.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/security/diebold-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Banking
- Retail
- ATM
- Self-Service
- Point of Sale
- Fortune 1000
---
