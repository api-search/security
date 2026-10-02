---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: temlavo.com
  spf: true
hosts:
- cert_expires: Dec 18 18:56:12 2026 GMT
  host: temlavo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Temlavo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temlavo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Temlavo
provider_slug: temlavo
slug: temlavo-domain-security
source_filename: temlavo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: temlavo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 18:56:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: temlavo.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temlavo/refs/heads/main/security/temlavo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Invoice
- Extraction
- API
- Accounting
---
