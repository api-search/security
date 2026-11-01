---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: loopingagent.com
  spf: false
hosts:
- cert_expires: Jan 21 06:42:02 2027 GMT
  host: loopingagent.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Loopingagent Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for loopingagent-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: loopingagent-com
provider_slug: loopingagent-com
slug: loopingagent-com-domain-security
source_filename: loopingagent-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loopingagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 06:42:02 2027 GMT\n  hsts: false\ndomains:\n- domain: loopingagent.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/loopingagent-com/security/loopingagent-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Personal
- Portfolio
- AI
- Consulting
- Software
---
