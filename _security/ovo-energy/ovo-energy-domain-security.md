---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "www.digicert.com; cansignhttpexchanges=yes"
  - 0 iodef "mailto:admin@ovo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ovoenergy.com
  spf: true
- caa:
  - 0 issuewild "www.digicert.com; cansignhttpexchanges=yes"
  - 0 iodef "mailto:admin@ovo.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "www.digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ovo.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.ovoenergy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 20:20:58 2026 GMT
  host: api.ovoenergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 04:18:55 2026 GMT
  host: my.ovoenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 15:32:55 2026 GMT
  host: smartpaymapi.ovoenergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: forum.ovoenergy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:02:52 2026 GMT
  host: account.ovoenergy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 19:43:10 2026 GMT
  host: company.ovo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 19:53:42 2026 GMT
  host: careers.ovo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ovo Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OVO Energy, probed live across 8 host(s) and 2 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OVO Energy
provider_slug: ovo-energy
slug: ovo-energy-domain-security
source_filename: ovo-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ovoenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ovoenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:20:58 2026 GMT\n  hsts: null\n- host: my.ovoenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:18:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: smartpaymapi.ovoenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:32:55 2026 GMT\n  hsts: null\n- host: forum.ovoenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: account.ovoenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:02:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: company.ovo.com\n \
  \ https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:43:10 2026 GMT\n  hsts: false\n- host: careers.ovo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 19:53:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ovoenergy.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"www.digicert.com; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:admin@ovo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ovo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"www.digicert.com; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:admin@ovo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"www.digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"\
  amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ovo-energy/refs/heads/main/security/ovo-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Energy Retail
- Solar
- EV Charging
- Demand Response
---
