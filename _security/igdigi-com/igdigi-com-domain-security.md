---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@igdigi.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: igdigi.com
  spf: true
hosts:
- cert_expires: Jan 26 21:55:46 2027 GMT
  host: igdigi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IG Digital Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IG Digital Lab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: IG Digital Lab
provider_slug: igdigi-com
slug: igdigi-com-domain-security
source_filename: igdigi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: igdigi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 21:55:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: igdigi.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@igdigi.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/igdigi-com/security/igdigi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Software Development
- AI Automation
- Web Development
- Mobile Development
- Call Center AI
- Workflow Automation
- IT Support
- Small Business Services
---
