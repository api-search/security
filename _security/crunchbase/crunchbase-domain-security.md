---
api_specs:
- filename: crunchbase-openapi.yml
  format: yaml
  label: Crunchbase API
  slug: crunchbase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase/refs/heads/main/openapi/crunchbase-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crunchbase.com
  spf: true
hosts:
- cert_expires: Sep 12 15:01:53 2026 GMT
  host: www.crunchbase.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:58:43 2026 GMT
  host: data.crunchbase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.crunchbase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crunchbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crunchbase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crunchbase
provider_slug: crunchbase
slug: crunchbase-domain-security
source_filename: crunchbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crunchbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:01:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: data.crunchbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:58:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.crunchbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crunchbase.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchbase/refs/heads/main/security/crunchbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Data
- Funding
- Investments
- Startups
- Private Markets
- Firmographics
---
