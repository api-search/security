---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: useslop.com
  spf: false
hosts:
- cert_expires: Jan 14 11:24:04 2027 GMT
  host: useslop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Useslop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Useslop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Useslop
provider_slug: useslop-com
slug: useslop-com-domain-security
source_filename: useslop-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: useslop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 11:24:04 2027 GMT\n  hsts: null\ndomains:\n- domain: useslop.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/useslop-com/security/useslop-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
