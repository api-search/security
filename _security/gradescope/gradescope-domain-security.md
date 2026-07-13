---
api_specs:
- filename: gradescope-openapi.yml
  format: yaml
  label: Gradescope LTI Integration
  slug: gradescope-lti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradescope/refs/heads/main/openapi/gradescope-openapi.yml
- filename: gradescope-openapi.yml
  format: yaml
  label: Gradescope Courses API
  slug: gradescope-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradescope/refs/heads/main/openapi/gradescope-openapi.yml
- filename: gradescope-openapi.yml
  format: yaml
  label: Gradescope Assignments API
  slug: gradescope-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradescope/refs/heads/main/openapi/gradescope-openapi.yml
- filename: gradescope-openapi.yml
  format: yaml
  label: Gradescope Submissions API
  slug: gradescope-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradescope/refs/heads/main/openapi/gradescope-openapi.yml
- filename: gradescope-openapi.yml
  format: yaml
  label: Gradescope Grades API
  slug: gradescope-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradescope/refs/heads/main/openapi/gradescope-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:devops+caa@turnitin.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gradescope.com
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: www.gradescope.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 16 23:42:39 2026 GMT
  host: guides.gradescope.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: gradescope-autograders.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gradescope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gradescope, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gradescope
provider_slug: gradescope
slug: gradescope-domain-security
source_filename: gradescope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gradescope.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: false\n- host: guides.gradescope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:42:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gradescope-autograders.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gradescope.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:devops+caa@turnitin.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n \
  \ - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gradescope/refs/heads/main/security/gradescope-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- EdTech
- Grading
- Assessment
- LTI
---
