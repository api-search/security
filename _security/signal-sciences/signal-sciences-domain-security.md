---
description: ''
domains:
- caa:
  - 0 iodef "mailto:namecheap@signalsciences.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodo.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: signalsciences.com
  spf: true
- caa:
  - 0 iodef "mailto:security@fastly.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "amazonaws.com"
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fastly.com
  spf: true
hosts:
- host: www.signalsciences.com
  https: false
- cert_expires: Aug 15 21:22:03 2026 GMT
  host: www.fastly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  1 06:22:01 2026 GMT
  host: dashboard.signalsciences.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signal Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signal Sciences, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Signal Sciences
provider_slug: signal-sciences
slug: signal-sciences-domain-security
source_filename: signal-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.signalsciences.com\n  https: false\n- host: www.fastly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 21:22:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dashboard.signalsciences.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 06:22:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: signalsciences.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:namecheap@signalsciences.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodo.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fastly.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@fastly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf:\
  \ true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signal-sciences/refs/heads/main/security/signal-sciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Web Application Firewall
- WAF
- API Security
- RASP
- Application Security
- Bot Protection
---
