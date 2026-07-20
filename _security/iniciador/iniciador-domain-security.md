---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@iniciador.com.br"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: iniciador.com.br
  spf: true
hosts:
- cert_expires: Oct 16 23:12:42 2026 GMT
  host: iniciador.com.br
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:43:57 2026 GMT
  host: docs.iniciador.com.br
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 00:04:35 2026 GMT
  host: api.iniciador.com.br
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iniciador Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iniciador, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Iniciador
provider_slug: iniciador
slug: iniciador-domain-security
source_filename: iniciador-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iniciador.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:12:42 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.iniciador.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.iniciador.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:04:35 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: iniciador.com.br\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@iniciador.com.br\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iniciador/refs/heads/main/security/iniciador-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Open Finance
- Open Banking
- Payments
- Pix
- Brazil
- FAPI
- OAuth
- Financial Services
---
