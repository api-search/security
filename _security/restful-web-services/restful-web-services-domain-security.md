---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@postman.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postman.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swagger.io
  spf: true
hosts:
- cert_expires: Aug 16 09:00:12 2026 GMT
  host: www.postman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 16:46:01 2026 GMT
  host: swagger.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: spring.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Restful Web Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RESTful Web Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RESTful Web Services
provider_slug: restful-web-services
slug: restful-web-services-domain-security
source_filename: restful-web-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.postman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 09:00:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: swagger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:46:01 2026 GMT\n  hsts: false\n- host: spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: postman.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@postman.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: swagger.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restful-web-services/refs/heads/main/security/restful-web-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Architecture
- HTTP
- REST
- Web Services
---
