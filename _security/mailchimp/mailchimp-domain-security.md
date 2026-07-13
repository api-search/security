---
api_specs:
- filename: mailchimp-marketing-api-openapi.yml
  format: yaml
  label: Mailchimp Marketing API
  slug: mailchimp-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/openapi/mailchimp-marketing-api-openapi.yml
- filename: mailchimp-transactional-api-openapi.yml
  format: yaml
  label: Mailchimp Transactional API
  slug: mailchimp-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/openapi/mailchimp-transactional-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailchimp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mandrillapp.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: mailchimp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: server.api.mailchimp.com
  https: false
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: mandrillapp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mailchimp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailchimp, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mailchimp
provider_slug: mailchimp
slug: mailchimp-domain-security
source_filename: mailchimp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailchimp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: server.api.mailchimp.com\n  https: false\n- host: mandrillapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mailchimp.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mandrillapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/security/mailchimp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
---
