---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "microsoft.com"
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hotmail.com
  spf: true
hosts:
- cert_expires: Feb 27 18:55:07 2027 GMT
  host: hotmail.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hotmail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hotmail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hotmail
provider_slug: hotmail
slug: hotmail-domain-security
source_filename: hotmail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hotmail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 18:55:07 2027 GMT\n  hsts: null\ndomains:\n- domain: hotmail.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"microsoft.com\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotmail/refs/heads/main/security/hotmail-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email
- Webmail
- Consumer
- Communication
- Microsoft
- Legacy
- Messaging
---
