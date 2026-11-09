---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:info@fedlin.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fedlin.com
  spf: true
hosts:
- cert_expires: Feb  4 16:39:46 2027 GMT
  host: fedlin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fedlin Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FEDLIN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FEDLIN
provider_slug: fedlin-com
slug: fedlin-com-domain-security
source_filename: fedlin-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fedlin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 16:39:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fedlin.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:info@fedlin.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fedlin-com/security/fedlin-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Crypto-Agility
- Compliance
- Remote-Access
- Vulnerability-Remediation
---
