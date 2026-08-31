---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: thesim.dev
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:ssladmins@simcorp.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: simcorp.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: thesim.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 13:00:05 2026 GMT
  host: www.simcorp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simcorp Dimension Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimCorp Dimension, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SimCorp Dimension
provider_slug: simcorp-dimension
slug: simcorp-dimension-domain-security
source_filename: simcorp-dimension-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thesim.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\n- host: www.simcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:00:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thesim.dev\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n- domain: simcorp.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:ssladmins@simcorp.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simcorp-dimension/refs/heads/main/security/simcorp-dimension-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accounting
- Asset Management
- Compliance
- Data Distribution
- Enterprise Software
- Financial Data
- Financial Technology
- Investment Management
- Portfolio-Management
- Risk Management
- SimCorp One
- Streaming
- Trading
---
