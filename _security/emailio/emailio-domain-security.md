---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: emailio.com
  spf: false
hosts:
- cert_expires: Mar  5 11:00:34 2027 GMT
  host: www.emailio.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Emailio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emailio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Emailio
provider_slug: emailio
slug: emailio-domain-security
source_filename: emailio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emailio.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  5 11:00:34 2027 GMT\n  hsts: false\ndomains:\n- domain: emailio.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailio/refs/heads/main/security/emailio-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Email
- Email Client
- Productivity
- Health and Wellness
- Consumer
- Y Combinator
- Thiel Fellowship
---
