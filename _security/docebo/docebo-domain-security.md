---
api_specs:
- filename: developer.docebo.com
  format: yaml
  label: Docebo REST API
  slug: docebo-rest-api
  spec_type: OpenAPI
  url: https://developer.docebo.com
- filename: docebo-openapi-generated.yml
  format: yaml
  label: Docebo API
  slug: docebo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docebo/refs/heads/main/openapi/_ae-authored/docebo-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:devops@docebo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docebo.com
  spf: true
hosts:
- cert_expires: Dec 25 11:54:22 2026 GMT
  host: www.docebo.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 01:24:37 2026 GMT
  host: developer.docebo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Docebo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docebo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Docebo
provider_slug: docebo
slug: docebo-domain-security
source_filename: docebo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docebo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 11:54:22 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.docebo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 01:24:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: docebo.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:devops@docebo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docebo/refs/heads/main/security/docebo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LMS
- E-Learning
- Training
- Courses
- Certification
- Gamification
- Learning Plans
- Human Resources
- AI Learning
---
