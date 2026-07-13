---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:it@campusmgmt.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: anthology.com
  spf: true
- caa:
  - 128 issuewild "amazon.com"
  - 128 issuewild "digicert.com"
  - 128 issuewild "sectigo.com"
  - 128 iodef "mailto:dnstech@blackboard.com"
  - 128 issue "amazon.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: blackboard.com
  spf: true
hosts:
- cert_expires: Aug 28 23:57:14 2026 GMT
  host: www.anthology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: developer.blackboard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Blackboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blackboard, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Blackboard
provider_slug: blackboard
slug: blackboard-domain-security
source_filename: blackboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anthology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:57:14 2026 GMT\n  hsts: false\n- host: developer.blackboard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anthology.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:it@campusmgmt.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: blackboard.com\n  dnssec: true\n  caa:\n  - 128 issuewild \"amazon.com\"\n  - 128 issuewild \"digicert.com\"\n  - 128 issuewild \"sectigo.com\"\n  - 128 iodef \"mailto:dnstech@blackboard.com\"\n  - 128 issue \"amazon.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackboard/refs/heads/main/security/blackboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- EdTech
- LMS
- Learning Management
---
