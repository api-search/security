---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: compyl.com
  spf: true
hosts:
- cert_expires: Nov 18 07:47:09 2026 GMT
  host: compyl.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compyl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compyl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Compyl
provider_slug: compyl
slug: compyl-domain-security
source_filename: compyl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compyl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 07:47:09 2026 GMT\n  hsts: false\ndomains:\n- domain: compyl.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compyl/refs/heads/main/security/compyl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- GRC
- Artificial Intelligence
- Compliance
- Risk Management
---
