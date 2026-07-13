---
api_specs:
- filename: 72a32ca1-f3a2-4a5e-91f2-token
  format: yaml
  label: Postman API
  slug: postman-api
  spec_type: OpenAPI
  url: https://www.postman.com/postman/postman-public-workspace/api/72a32ca1-f3a2-4a5e-91f2-token
- filename: openapi.yaml
  format: yaml
  label: k6 Performance Testing
  slug: k6-performance-testing
  spec_type: OpenAPI
  url: https://grafana.com/docs/k6/latest/misc/k6-rest-api/
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@postman.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postman.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getpostman.com
  spf: true
hosts:
- cert_expires: Aug 16 09:00:12 2026 GMT
  host: www.postman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:02:05 2026 GMT
  host: api.getpostman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 04:49:50 2026 GMT
  host: rest-assured.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Test Scripts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Test Scripts, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Test Scripts
provider_slug: test-scripts
slug: test-scripts-domain-security
source_filename: test-scripts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.postman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 09:00:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getpostman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest-assured.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:49:50 2026 GMT\n  hsts: false\ndomains:\n- domain: postman.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@postman.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getpostman.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\
  \n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-scripts/refs/heads/main/security/test-scripts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- CI/CD
- Contract Testing
- Quality Assurance
- Software Development
- Testing
---
