---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ikeytz.com
  spf: true
hosts:
- cert_expires: Dec 20 13:33:07 2026 GMT
  host: ikeytz.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ikeytz Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ikeytz-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ikeytz-com
provider_slug: ikeytz-com
slug: ikeytz-com-domain-security
source_filename: ikeytz-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ikeytz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 13:33:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ikeytz.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ikeytz-com/security/ikeytz-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Locksmith
- Security
- EmergencyService
- Germany
- Ludwigsburg
---
