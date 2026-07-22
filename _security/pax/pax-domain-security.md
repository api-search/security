---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paxai.com
  spf: true
hosts:
- cert_expires: Oct 10 03:27:42 2026 GMT
  host: paxai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 09:19:21 2026 GMT
  host: api.paxai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pax, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pax
provider_slug: pax
slug: pax-domain-security
source_filename: pax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paxai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:27:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.paxai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 09:19:21 2026 GMT\n  hsts: null\ndomains:\n- domain: paxai.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pax/refs/heads/main/security/pax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Artificial Intelligence
- Trade Finance
- Customs
- Duty Drawback
- Tariffs
- Fintech
- Supply Chain
---
