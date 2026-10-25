---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: south32.net
  spf: true
hosts:
- cert_expires: Jan 14 05:38:38 2027 GMT
  host: south32.net
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: South32 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for South32, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: South32
provider_slug: south32
slug: south32-domain-security
source_filename: south32-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: south32.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 05:38:38 2027 GMT\n  hsts: null\ndomains:\n- domain: south32.net\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/south32/refs/heads/main/security/south32-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Mining
- Metals
- Aluminium
- Australia
- Natural Resources
---
