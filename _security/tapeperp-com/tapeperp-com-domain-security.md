---
api_specs:
- filename: tapeperp-com-free-api-openapi.yml
  format: yaml
  label: Tape Free API
  slug: tapeperp-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapeperp-com/openapi/tapeperp-com-free-api-openapi.yml
- filename: tapeperp-com-paid-api-openapi.yml
  format: yaml
  label: Tape Paid API
  slug: tapeperp-com-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapeperp-com/openapi/tapeperp-com-paid-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@tapeperp.com"
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: true
  domain: tapeperp.com
  spf: true
hosts:
- cert_expires: Feb 12 07:09:20 2027 GMT
  host: tapeperp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tape, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tape
provider_slug: tapeperp-com
slug: tapeperp-com-domain-security
source_filename: tapeperp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tapeperp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 07:09:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tapeperp.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@tapeperp.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tapeperp-com/security/tapeperp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Cryptocurrency
- MarketData
- RealTime
- Finance
---
