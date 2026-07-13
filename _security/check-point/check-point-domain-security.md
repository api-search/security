---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:hostmaster@checkpoint.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issuewild "godaddy.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: checkpoint.com
  spf: true
hosts:
- cert_expires: Jan  2 06:44:08 2027 GMT
  host: www.checkpoint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: sc1.checkpoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Check Point Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Check Point Software, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Check Point Software
provider_slug: check-point
slug: check-point-domain-security
source_filename: check-point-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 06:44:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sc1.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: checkpoint.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:hostmaster@checkpoint.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/check-point/refs/heads/main/security/check-point-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Cybersecurity
- Firewall
- Network Security
- Cloud Security
- Endpoint Security
- Threat Intelligence
---
