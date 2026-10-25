---
description: ''
domains:
- caa:
  - 0 issue "cloudflare.com"
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazontrust.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: premierinc.com
  spf: true
hosts:
- cert_expires: Jan  5 19:13:47 2027 GMT
  host: www.premierinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.premierinc.com
  https: false
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: api.premierinc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Premier Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Premier Inc, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Premier Inc
provider_slug: premier-inc
slug: premier-inc-domain-security
source_filename: premier-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.premierinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:13:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.premierinc.com\n  https: false\n- host: api.premierinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: premierinc.com\n  dnssec: false\n  caa:\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/premier-inc/refs/heads/main/security/premier-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Group Purchasing
- Analytics
- Supply Chain
- Value-Based Care
---
