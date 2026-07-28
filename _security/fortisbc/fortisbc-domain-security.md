---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fortisbc.com
  spf: true
hosts:
- cert_expires: Sep 19 20:01:02 2026 GMT
  host: www.fortisbc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: accounts.fortisbc.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 157680000
  https: true
  note: Customer login (SiteMinder/SAML). Fronted by a Citrix NetScaler application firewall that answers unknown paths with a soft 200 block page.
  tls_version: TLSv1.3
- host: outages.fortisbc.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 157680000
  https: true
  note: Outage map. Same NetScaler application firewall as accounts.
  tls_version: TLSv1.3
- host: rebates.fortisbc.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fortisbc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FortisBC, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FortisBC
provider_slug: fortisbc
slug: fortisbc-domain-security
source_filename: fortisbc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (probe-domain-security.py),\n  extended by hand with the accounts./outages./rebates. subdomains probed\n  2026-07-27\nhosts:\n- host: www.fortisbc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:01:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: accounts.fortisbc.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 157680000\n  hsts_include_subdomains: true\n  note: >-\n    Customer login (SiteMinder/SAML). Fronted by a Citrix NetScaler application\n    firewall that answers unknown paths with a soft 200 block page.\n- host: outages.fortisbc.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 157680000\n  hsts_include_subdomains: true\n  note: Outage map. Same NetScaler application firewall as accounts.\n- host: rebates.fortisbc.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age:\
  \ 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  server: cloudflare\ndomains:\n- domain: fortisbc.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortisbc/refs/heads/main/security/fortisbc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Canada
- Utilities
- Electricity
- Natural Gas
- Gas Distribution
- Smart Metering
- Renewables
- EV Charging
- LNG
---
