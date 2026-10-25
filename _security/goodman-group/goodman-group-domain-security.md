---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goodman.com
  spf: true
hosts:
- cert_expires: Dec  6 05:14:18 2026 GMT
  host: goodman.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Goodman Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goodman Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Goodman Group
provider_slug: goodman-group
slug: goodman-group-domain-security
source_filename: goodman-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goodman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 05:14:18 2026 GMT\n  hsts: null\ndomains:\n- domain: goodman.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodman-group/refs/heads/main/security/goodman-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Industrial Property
- Real Estate
- Logistics
- Data Centers
- Property Development
- Funds Management
- Australia
---
