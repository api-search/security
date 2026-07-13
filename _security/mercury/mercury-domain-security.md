---
api_specs:
- filename: mercury-webhooks-asyncapi.yml
  format: yaml
  label: Mercury Webhooks API
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/asyncapi/mercury-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mercury.com
  spf: true
hosts:
- cert_expires: Sep 24 01:14:04 2026 GMT
  host: mercury.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:12:08 2026 GMT
  host: docs.mercury.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 01:14:04 2026 GMT
  host: api.mercury.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercury Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercury, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mercury
provider_slug: mercury
slug: mercury-domain-security
source_filename: mercury-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mercury.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 01:14:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mercury.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:12:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mercury.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 01:14:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mercury.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercury/refs/heads/main/security/mercury-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Fintech
- Startups
- Treasury
- Payments
---
