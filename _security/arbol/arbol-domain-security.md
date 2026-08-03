---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arbol.io
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: arbol.uk
  spf: false
hosts:
- cert_expires: Oct  1 11:52:44 2026 GMT
  host: www.arbol.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 13:20:03 2026 GMT
  host: insurance.arbol.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 00:44:23 2026 GMT
  host: insurance.arbol.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: app.arbol.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arbol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arbol, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Arbol
provider_slug: arbol
slug: arbol-domain-security
source_filename: arbol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arbol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:52:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: insurance.arbol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:20:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: insurance.arbol.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 00:44:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.arbol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: arbol.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: arbol.uk\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\nx-note: >-\n  www.arbol.io was probed by 0-working/probe-domain-security.py from apis.yml\n  hosts; insurance.arbol.io, insurance.arbol.uk\
  \ and app.arbol.io were probed\n  manually on the same date because Arbol has no apis[] entries for the script\n  to walk. app.arbol.io — the authenticated broker/agent platform — is the one\n  host with no HSTS header. arbol.uk publishes no SPF or DMARC record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbol/refs/heads/main/security/arbol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- Parametric Insurance
- Climate Risk
- Weather
- Reinsurance
- Climate Data
- Agriculture
- Energy
- Risk Management
---
