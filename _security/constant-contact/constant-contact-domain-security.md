---
api_specs:
- filename: swagger.yaml
  format: yaml
  label: Constant Contact V3 API
  slug: v3
  spec_type: OpenAPI
  url: https://api.cc.email/v3/swagger.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: constantcontact.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cc.email
  spf: true
hosts:
- cert_expires: Aug 29 06:27:16 2026 GMT
  host: www.constantcontact.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: developer.constantcontact.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: api.cc.email
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Constant Contact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constant Contact, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Constant Contact
provider_slug: constant-contact
slug: constant-contact-domain-security
source_filename: constant-contact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.constantcontact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:27:16 2026 GMT\n  hsts: null\n- host: developer.constantcontact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: false\n- host: api.cc.email\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: constantcontact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cc.email\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/security/constant-contact-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Campaigns
- Contacts
- Email Marketing
- Events
- Reporting
- SMS
- Surveys
---
