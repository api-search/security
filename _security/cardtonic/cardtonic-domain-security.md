---
api_specs:
- filename: cardtonic-openapi.yml
  format: yaml
  label: Cardtonic Business API
  slug: business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardtonic/refs/heads/main/openapi/cardtonic-openapi.yml
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
  domain: cardtonic.com
  spf: true
hosts:
- cert_expires: Dec  2 15:02:59 2026 GMT
  host: cardtonic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 15:02:59 2026 GMT
  host: api.cardtonic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Cardtonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardtonic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cardtonic
provider_slug: cardtonic
slug: cardtonic-domain-security
source_filename: cardtonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cardtonic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 15:02:59 2026 GMT\n  hsts: false\n- host: api.cardtonic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 15:02:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cardtonic.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardtonic/refs/heads/main/security/cardtonic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Africa
- Bill Payments
- eSIM
- Finance
- Fintech
- Gift Cards
- Ghana
- Nigeria
- Payments
- Virtual Dollar Cards
---
