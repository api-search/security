---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aceable.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aceableagent.com
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: www.aceable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:53:11 2026 GMT
  host: app.aceable.com
  hsts: false
  https: true
  note: student course application (single-page app; returns HTTP 200 HTML for every path, including /.well-known/*)
  tls_version: TLSv1.3
- cert_expires: Oct 11 02:04:43 2026 GMT
  host: api.aceable.com
  hsts: false
  https: true
  note: private platform API (Express on Heroku); every probed path returns HTTP 401 "Cannot Authorize Application ID" (code 40100)
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: www.aceableagent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: insurance.aceable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: mortgage.aceable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 16:30:59 2026 GMT
  host: partnerships.aceable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aceable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aceable, probed live across 7 host(s) and 2 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aceable
provider_slug: aceable
slug: aceable-domain-security
source_filename: aceable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + observed Aceable Brands hosts\nhosts:\n- host: www.aceable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.aceable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:53:11 2026 GMT\n  hsts: false\n  note: student course application (single-page app; returns HTTP 200 HTML for every\n    path, including /.well-known/*)\n- host: api.aceable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 02:04:43 2026 GMT\n  hsts: false\n  note: private platform API (Express on Heroku); every probed path returns HTTP 401\n    \"Cannot Authorize Application ID\" (code 40100)\n- host: www.aceableagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: insurance.aceable.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mortgage.aceable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partnerships.aceable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 16:30:59 2026 GMT\n  hsts: false\ndomains:\n- domain: aceable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aceableagent.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nfindings:\n- All public marketing hosts serve TLS 1.3 and set HSTS with a one-year max-age; the\n  application host (app.aceable.com), the API host (api.aceable.com) and the partner\n  marketing host (partnerships.aceable.com) do not set HSTS.\n- Neither aceable.com nor aceableagent.com is DNSSEC-signed.\n-\
  \ aceable.com publishes no CAA record; aceableagent.com pins issuance to Let's Encrypt,\n  Amazon and DigiCert.\n- Both registrable domains publish SPF and DMARC at p=quarantine (not reject).\n- No /.well-known/security.txt is served on any Aceable host and no vulnerability\n  disclosure or bug bounty program was found (see well-known/aceable-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aceable/refs/heads/main/security/aceable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Online Learning
- Continuing Education
- Licensing
- Certification
- Drivers Education
- Real-Estate
- Insurance
- Mortgage
- Compliance Training
- Austin
---
