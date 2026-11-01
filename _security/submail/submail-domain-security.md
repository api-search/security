---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mysubmail.com
  spf: true
hosts:
- cert_expires: Mar 25 23:59:59 2027 GMT
  host: www.mysubmail.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Submail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SUBMAIL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SUBMAIL
provider_slug: submail
slug: submail-domain-security
source_filename: submail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mysubmail.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mysubmail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/submail/security/submail-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
