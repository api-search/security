---
api_specs:
- filename: email-on-acid-openapi.yml
  format: yaml
  label: Email on Acid API
  slug: email-on-acid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/email-on-acid/refs/heads/main/openapi/email-on-acid-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: emailonacid.com
  spf: true
hosts:
- cert_expires: Sep 17 22:47:01 2026 GMT
  host: www.emailonacid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: api.emailonacid.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Email On Acid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Email on Acid, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Email on Acid
provider_slug: email-on-acid
slug: email-on-acid-domain-security
source_filename: email-on-acid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emailonacid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:47:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.emailonacid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: emailonacid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/email-on-acid/refs/heads/main/security/email-on-acid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Testing
- Email Previews
- Email Clients
- Spam Testing
- Accessibility
- HTML Validation
- Email Quality Assurance
- Pre-Deployment Testing
---
