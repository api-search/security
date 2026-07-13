---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: certero.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: servicenow.com
  spf: true
hosts:
- cert_expires: Sep  9 10:36:19 2026 GMT
  host: www.certero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 08:31:45 2026 GMT
  host: store.servicenow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Certero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certero, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Certero
provider_slug: certero
slug: certero-domain-security
source_filename: certero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.certero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 10:36:19 2026 GMT\n  hsts: false\n- host: store.servicenow.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 08:31:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: certero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: servicenow.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certero/refs/heads/main/security/certero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Management
- FinOps
- Hardware Asset Management
- IT Asset Management
- ITAM
- License Management
- SaaS Management
- Software Asset Management
- Software Licensing
---
