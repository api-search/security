---
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nerc.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nerc.net
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eisac.com
  note: E-ISAC domain, added by hand on 2026-07-27 (the automated probe walks the apis.yml + OpenAPI hosts and had captured the www.eisac.com host but not the registrable domain). SPF includes _spf.salesforce.com, cust-spf.exacttarget.com, mmsend.com and spf.protection.outlook.com with -all; DMARC p=quarantine pct=100 with rua/ruf reporting.
  spf: true
hosts:
- cert_expires: Sep 25 22:28:40 2026 GMT
  host: www.nerc.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 03:37:32 2026 GMT
  host: eroportal.nerc.net
  hsts: true
  hsts_max_age: 3153600
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: www.eisac.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nerc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NERC, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NERC
provider_slug: nerc
slug: nerc-domain-security
source_filename: nerc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nerc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:28:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: eroportal.nerc.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 03:37:32 2026 GMT\n  hsts: true\n  hsts_max_age: 3153600\n- host: www.eisac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nerc.com\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nerc.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog;\
  \ cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: eisac.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  note: >-\n    E-ISAC domain, added by hand on 2026-07-27 (the automated probe walks the\n    apis.yml + OpenAPI hosts and had captured the www.eisac.com host but not the\n    registrable domain). SPF includes _spf.salesforce.com, cust-spf.exacttarget.com,\n\
  \    mmsend.com and spf.protection.outlook.com with -all; DMARC p=quarantine\n    pct=100 with rua/ruf reporting.\nfindings:\n  dnssec: Not enabled on nerc.com, nerc.net or eisac.com.\n  hsts: Enabled on all three probed hosts; www.eisac.com carries the longest max-age\n    (63072000, two years).\n  caa: All three domains publish CAA issue records, constraining certificate issuance.\n  email: SPF and DMARC published on all three domains; nerc.com and eisac.com enforce\n    p=quarantine, nerc.net is p=none (monitor only).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nerc/refs/heads/main/security/nerc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Canada
- Electricity
- Grid
- Regulator
- Government
- Reliability
- Bulk Power System
- Critical Infrastructure
- Cyber Security
- Energy Markets
- Compliance
---
