---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: postfix.org
  spf: true
hosts:
- cert_expires: Sep 14 03:46:30 2026 GMT
  host: www.postfix.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postfix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postfix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Postfix
provider_slug: postfix
slug: postfix-domain-security
source_filename: postfix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.postfix.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:46:30 2026 GMT\n  hsts: false\ndomains:\n- domain: postfix.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postfix/refs/heads/main/security/postfix-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Email
- Mail Server
- MTA
- SMTP
- Open Source
- Infrastructure
---
