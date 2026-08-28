---
api_specs:
- filename: paubox-email-api-openapi.yaml
  format: yaml
  label: Paubox Email API
  slug: paubox-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-email-api-openapi.yaml
- filename: paubox-marketing-api-openapi.yaml
  format: yaml
  label: Paubox Marketing API
  slug: paubox-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-marketing-api-openapi.yaml
- filename: paubox-forms-api-openapi.yaml
  format: yaml
  label: Paubox Forms API
  slug: paubox-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/openapi/paubox-forms-api-openapi.yaml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:security@paubox.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paubox.com
  spf: true
hosts:
- cert_expires: Nov 17 22:03:40 2026 GMT
  host: www.paubox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 18:44:00 2026 GMT
  host: docs.paubox.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.paubox.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Paubox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paubox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paubox
provider_slug: paubox
slug: paubox-domain-security
source_filename: paubox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paubox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 22:03:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.paubox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 18:44:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.paubox.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: paubox.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:security@paubox.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paubox/refs/heads/main/security/paubox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- HIPAA
- Healthcare
- Compliance
- Transactional Email
- Email Marketing
- Forms
- Security
- Encryption
- Messaging
---
