---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "fnmt.es"
  - 0 issue "visa.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "buypass.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: revolut.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "buypass.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: monzo.com
  spf: true
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: developer.revolut.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: api.revolut.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 02:45:32 2026 GMT
  host: docs.monzo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neobanks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neobanks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Neobanks
provider_slug: neobanks
slug: neobanks-domain-security
source_filename: neobanks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.revolut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.revolut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\n- host: docs.monzo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:45:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: revolut.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"fnmt.es\"\n  - 0 issue \"visa.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"buypass.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: monzo.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"buypass.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\
  \n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neobanks/refs/heads/main/security/neobanks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Digital Banking
- Fintech
- Mobile Banking
- Neobank
- Open Banking
---
