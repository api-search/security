---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:hostmaster@myemma.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: myemma.com
  spf: true
hosts:
- cert_expires: Jan 11 21:14:36 2027 GMT
  host: myemma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Myemma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Emma
provider_slug: myemma
slug: myemma-domain-security
source_filename: myemma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myemma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 21:14:36 2027 GMT\n  hsts: false\ndomains:\n- domain: myemma.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:hostmaster@myemma.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/myemma/security/myemma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Marketing
- Automation
- AI
- SMS
- Higher Education
- Nonprofit
- Government
- Travel & Hospitality
---
