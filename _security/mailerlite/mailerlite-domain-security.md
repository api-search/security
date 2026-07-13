---
api_specs:
- filename: mailerlite-openapi.yml
  format: yaml
  label: MailerLite API
  slug: mailerlite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailerlite.com
  spf: true
hosts:
- cert_expires: Sep 15 09:56:40 2026 GMT
  host: www.mailerlite.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 11:35:40 2026 GMT
  host: developers.mailerlite.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 09:56:40 2026 GMT
  host: connect.mailerlite.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mailerlite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MailerLite, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MailerLite
provider_slug: mailerlite
slug: mailerlite-domain-security
source_filename: mailerlite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mailerlite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:56:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.mailerlite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:35:40 2026 GMT\n  hsts: false\n- host: connect.mailerlite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:56:40 2026 GMT\n  hsts: false\ndomains:\n- domain: mailerlite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/security/mailerlite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- Automation
- Newsletters
- Subscribers
---
