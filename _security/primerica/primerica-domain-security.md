---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: primerica.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: primericaonline.com
  spf: true
hosts:
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: www.primerica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: gtw.primericaonline.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Primerica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Primerica, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Primerica
provider_slug: primerica
slug: primerica-domain-security
source_filename: primerica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.primerica.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: gtw.primericaonline.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: primerica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: primericaonline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primerica/refs/heads/main/security/primerica-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Insurance
- Financial-Services
- Life Insurance
- Identity
- Authentication
- OpenID Connect
- API Gateway
---
