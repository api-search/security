---
description: ''
domains:
- caa:
  - 0 issue "Digicert.com"
  - 0 issue "telesec.de"
  - 0 issuewild "telesec.de"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "sectigo.com"
  dmarc: false
  dnssec: false
  domain: netid.de
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: netid.de
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for netID, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: netID
provider_slug: netid
slug: netid-domain-security
source_filename: netid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netid.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: netid.de\n  dnssec: false\n  caa:\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"telesec.de\"\n  - 0 issuewild \"telesec.de\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/netid/security/netid-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Identity
- Authentication
- Login
- German
---
