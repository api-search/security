---
api_specs:
- filename: tradify-openapi.yml
  format: yaml
  label: Tradify Jobs API (Modeled)
  slug: tradify-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/openapi/tradify-openapi.yml
- filename: tradify-openapi.yml
  format: yaml
  label: Tradify Customers API (Modeled)
  slug: tradify-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/openapi/tradify-openapi.yml
- filename: tradify-openapi.yml
  format: yaml
  label: Tradify Quotes API (Modeled)
  slug: tradify-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/openapi/tradify-openapi.yml
- filename: tradify-openapi.yml
  format: yaml
  label: Tradify Invoices API (Modeled)
  slug: tradify-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/openapi/tradify-openapi.yml
- filename: tradify-openapi.yml
  format: yaml
  label: Tradify Timesheets API (Modeled)
  slug: tradify-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/openapi/tradify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:dmarc@tradifyhq.com; ruf=mailto:dmarc@tradifyhq.com;
  dnssec: false
  domain: tradifyhq.com
  nameservers:
  - hayes.ns.cloudflare.com
  - imani.ns.cloudflare.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:2929749.spf10.hubspotemail.net include:spf.mandrillapp.com include:mail.zendesk.com -all
hosts:
- cert_expires: Sep 12 01:02:51 2026 GMT
  host: www.tradifyhq.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  notes: Marketing site served via HubSpot CMS behind Cloudflare.
  tls_issuer: Google Trust Services (WE1)
- host: tradifyhq.com
  hsts: null
  https: true
  notes: Apex 301-redirects to www; ASP.NET / IIS front responds before redirect.
  redirect: https://www.tradifyhq.com/
  server: Microsoft-IIS/10.0
- cert_expires: Sep  7 22:39:52 2026 GMT
  csp: default-src 'none'; script-src 'self'; connect-src 'self'; img-src 'self'; style-src 'self'; base-uri 'self'; form-action 'self'
  host: api.tradifyhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  notes: Live application backend (HTTP 200, empty body at root). Undocumented and session-authenticated - used by Tradify's own web/mobile apps, NOT a public API. Locked-down CSP (default-src 'none'). TLS cert issuer differs from the marketing site, confirming a separate origin.
  tls_issuer: GoDaddy Secure Certificate Authority - G2
  x_content_type_options: nosniff
- host: help.tradifyhq.com
  hsts: true
  hsts_max_age: 259200
  https: true
  notes: Zendesk-hosted help centre.
  server: cloudflare
kind: domain-security
layout: security
method: probed
name: Tradify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tradify, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tradify
provider_slug: tradify
slug: tradify-domain-security
source_filename: tradify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of Tradify hosts (apis.yml + known app backend)\nhosts:\n- host: www.tradifyhq.com\n  https: true\n  tls_issuer: Google Trust Services (WE1)\n  cert_expires: Sep 12 01:02:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  notes: Marketing site served via HubSpot CMS behind Cloudflare.\n- host: tradifyhq.com\n  https: true\n  redirect: https://www.tradifyhq.com/\n  server: Microsoft-IIS/10.0\n  hsts: null\n  notes: Apex 301-redirects to www; ASP.NET / IIS front responds before redirect.\n- host: api.tradifyhq.com\n  https: true\n  tls_issuer: GoDaddy Secure Certificate Authority - G2\n  cert_expires: Sep  7 22:39:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  csp: \"default-src 'none'; script-src 'self'; connect-src 'self'; img-src 'self'; style-src 'self'; base-uri 'self'; form-action 'self'\"\n  x_content_type_options: nosniff\n  notes:\
  \ >-\n    Live application backend (HTTP 200, empty body at root). Undocumented and\n    session-authenticated - used by Tradify's own web/mobile apps, NOT a public\n    API. Locked-down CSP (default-src 'none'). TLS cert issuer differs from the\n    marketing site, confirming a separate origin.\n- host: help.tradifyhq.com\n  https: true\n  server: cloudflare\n  hsts: true\n  hsts_max_age: 259200\n  notes: Zendesk-hosted help centre.\ndomains:\n- domain: tradifyhq.com\n  dnssec: false\n  nameservers:\n  - hayes.ns.cloudflare.com\n  - imani.ns.cloudflare.com\n  caa: []\n  spf: true\n  spf_record: \"v=spf1 include:_spf.google.com include:sendgrid.net include:2929749.spf10.hubspotemail.net include:spf.mandrillapp.com include:mail.zendesk.com -all\"\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: \"v=DMARC1; p=none; rua=mailto:dmarc@tradifyhq.com; ruf=mailto:dmarc@tradifyhq.com;\"\nobservations:\n- All probed public hosts serve HTTPS with HSTS enabled.\n- No CAA records are published\
  \ on tradifyhq.com (multiple CAs observed across hosts - Google Trust Services and GoDaddy).\n- DMARC is published but policy is p=none (monitor only), so spoofed mail is not actively rejected/quarantined.\n- SPF ends in -all (hard fail) and enumerates Google, SendGrid, HubSpot, Mandrill, and Zendesk as authorized senders.\n- No public API host or developer surface was found to probe; api.tradifyhq.com is the app backend and is undocumented.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradify/refs/heads/main/security/tradify-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Job Management
- Trades
- Field Service
- Scheduling
- Quoting
- Invoicing
- Timesheets
- Contractors
- SaaS
---
