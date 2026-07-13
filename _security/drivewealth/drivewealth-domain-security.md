---
api_specs:
- filename: dw-openapi
  format: yaml
  label: DriveWealth REST API
  slug: drivewealth-rest-api
  spec_type: OpenAPI
  url: https://github.com/DriveWealth/dw-openapi
description: ''
domains:
- caa:
  - 0 issue "digicert.net"
  - 0 issue "entrust.net"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 iodef "mailto:securitydisclosure@drivewealth.tech"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: drivewealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: drivewealth.net
  spf: false
hosts:
- cert_expires: Oct  4 04:08:29 2026 GMT
  host: drivewealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:21:56 2026 GMT
  host: developer.drivewealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.drivewealth.net
  https: false
kind: domain-security
layout: security
method: probed
name: Drivewealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DriveWealth, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DriveWealth
provider_slug: drivewealth
slug: drivewealth-domain-security
source_filename: drivewealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drivewealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:08:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.drivewealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:21:56 2026 GMT\n  hsts: null\n- host: api.drivewealth.net\n  https: false\ndomains:\n- domain: drivewealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.net\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:securitydisclosure@drivewealth.tech\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: drivewealth.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drivewealth/refs/heads/main/security/drivewealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Brokerage-as-a-Service
- Embedded Investing
- Fractional Shares
- Trading
- Fintech
- Equities
- ETFs
- Options
- Fixed Income
- Mutual Funds
- Portfolio Management
- Account Opening
- KYC
- Financial Services
---
