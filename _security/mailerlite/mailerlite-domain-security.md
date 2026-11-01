---
api_specs:
- filename: mailerlite-webhook-api-openapi.yml
  format: yaml
  label: MailerLite Webhook API
  slug: mailerlite-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailerlite/openapi/mailerlite-webhook-api-openapi.yml
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
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 11:46:24 2026 GMT
  host: developers.mailerlite.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: classic.developers.mailerlite.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Mailerlite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MailerLite, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MailerLite
provider_slug: mailerlite
slug: mailerlite-domain-security
source_filename: mailerlite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mailerlite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:56:40 2026 GMT\n  hsts: null\n- host: developers.mailerlite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 11:46:24 2026 GMT\n  hsts: false\n- host: classic.developers.mailerlite.com\n  https: false\ndomains:\n- domain: mailerlite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mailerlite/security/mailerlite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Marketing
- Automation
- Newsletters
- Subscribers
- Campaigns
- Webhook
- E-Commerce
- Segmentation
- Transactional Email
- MCP
- Email
---
