---
api_specs:
- filename: kaseya-bms-openapi-original.json
  format: json
  label: Kaseya BMS API 2.0
  slug: bms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaseya/refs/heads/main/openapi/kaseya-bms-openapi-original.json
- filename: kaseya-autotask-psa-openapi-original.json
  format: json
  label: Datto Autotask PSA REST API
  slug: autotask-psa
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaseya/refs/heads/main/openapi/kaseya-autotask-psa-openapi-original.json
- filename: kaseya-datto-rmm-openapi-original.json
  format: json
  label: Datto RMM API v2
  slug: datto-rmm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaseya/refs/heads/main/openapi/kaseya-datto-rmm-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kaseya.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: autotask.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: centrastage.net
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: itglue.com
  spf: true
- caa:
  - 0 issue "Digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datto.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myitprocess.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vsax.net
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.kaseya.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: help.bms.kaseya.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 10:48:07 2026 GMT
  host: api.bms.kaseya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: webservices2.autotask.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: syrah-api.centrastage.net
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.itglue.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: rmm.datto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: reporting.live.myitprocess.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 14:46:54 2026 GMT
  host: status.kaseya.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: one.kaseya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kaseya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaseya, probed live across 10 host(s) and 7 registrable domain(s). 10 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kaseya
provider_slug: kaseya
slug: kaseya-domain-security
source_filename: kaseya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kaseya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: help.bms.kaseya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\n- host: api.bms.kaseya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 10:48:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webservices2.autotask.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: syrah-api.centrastage.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\n- host: api.itglue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\n- host: rmm.datto.com\n  https: true\n  tls_version: TLSv1.3\n\
  \  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n- host: reporting.live.myitprocess.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\n- host: status.kaseya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 14:46:54 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: one.kaseya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kaseya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: autotask.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: centrastage.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: itglue.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n\
  \  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: datto.com\n  dnssec: false\n  caa:\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: myitprocess.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: vsax.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaseya/refs/heads/main/security/kaseya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IT Management
- Managed Service Providers
- Remote Monitoring and Management
- Professional Services Automation
- Cybersecurity
- Backup and Disaster Recovery
- IT Documentation
- Endpoint Management
- Service Desk
- Ticketing
- Compliance
---
