---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bespokepost.com
  spf: true
hosts:
- cert_expires: Oct 16 23:20:42 2026 GMT
  host: bespokepost.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nabfly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nabfly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: nabfly
provider_slug: nabfly
slug: nabfly-domain-security
source_filename: nabfly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bespokepost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:20:42 2026 GMT\n  hsts: null\ndomains:\n- domain: bespokepost.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nabfly/refs/heads/main/security/nabfly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ecommerce
- Retail
- Subscription
- Consumer
- Direct-to-Consumer
- Menswear
- Lifestyle
---
