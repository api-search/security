---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: console.com.au
  spf: true
hosts:
- cert_expires: Oct  1 12:50:36 2026 GMT
  host: www.console.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.console.com.au
  hsts: false
  http_status: 404
  https: true
  note: Kong API Gateway behind nginx; no route exposed anonymously, no HSTS header.
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: app.console.com.au
  hsts: false
  http_status: 307
  https: true
  note: Redirects to pm.reapit.com.au (Reapit PM application host).
  tls_version: TLSv1.3
- cert_expires: Oct  4 04:27:38 2026 GMT
  host: my.console.com.au
  hsts: false
  http_status: 301
  https: true
  note: Redirects to myconsole.com.au; Cloudflare-fronted.
  tls_version: TLSv1.3
- cert_expires: Sep 18 20:32:03 2026 GMT
  host: go.console.com.au
  hsts: false
  http_status: 302
  https: true
  note: Marketo landing-page host (console.mktoweb.com).
  tls_version: TLSv1.3
- host: help.console.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  http_status: 301
  https: true
  note: 'Salesforce Experience Cloud help centre (…live.siteforce.com). TLS handshake could

    not be verified from the probing host (local CA chain), but HTTPS requests succeed

    and the strongest HSTS policy on any Console host is served here.

    '
  tls_version: null
- host: status.console.com.au
  hsts: false
  http_status: 200
  https: true
  note: Hund.io status page (CNAME console.hund.io).
- host: sso.console.com.au
  hsts: false
  http_status: 301
  https: true
  note: Cloudflare; 301 to login.console.com.au, which resolves but does not answer HTTPS.
kind: domain-security
layout: security
method: probed
name: Console Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Console Group, probed live across 8 host(s) and 1 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Console Group
provider_slug: console-group
slug: console-group-domain-security
source_filename: console-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: |\n  live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (0-working/probe-domain-security.py),\n  extended by a manual subdomain sweep and per-host TLS/HSTS probe on 2026-07-26\nhosts:\n- host: www.console.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:50:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.console.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\n  http_status: 404\n  note: Kong API Gateway behind nginx; no route exposed anonymously, no HSTS header.\n- host: app.console.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\n  http_status: 307\n  note: Redirects to pm.reapit.com.au (Reapit PM application host).\n- host: my.console.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:27:38 2026 GMT\n  hsts: false\n  http_status: 301\n  note: Redirects\
  \ to myconsole.com.au; Cloudflare-fronted.\n- host: go.console.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:32:03 2026 GMT\n  hsts: false\n  http_status: 302\n  note: Marketo landing-page host (console.mktoweb.com).\n- host: help.console.com.au\n  https: true\n  tls_version: null\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  http_status: 301\n  note: |\n    Salesforce Experience Cloud help centre (…live.siteforce.com). TLS handshake could\n    not be verified from the probing host (local CA chain), but HTTPS requests succeed\n    and the strongest HSTS policy on any Console host is served here.\n- host: status.console.com.au\n  https: true\n  http_status: 200\n  hsts: false\n  note: Hund.io status page (CNAME console.hund.io).\n- host: sso.console.com.au\n  https: true\n  http_status: 301\n  hsts: false\n  note: Cloudflare; 301 to login.console.com.au, which resolves but does not answer HTTPS.\ndomains:\n- domain: console.com.au\n\
  \  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/console-group/refs/heads/main/security/console-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Australia
- New Zealand
- Property Management
- PropTech
- Trust Accounting
- Rentals
- Tenancy
- Commercial Real Estate
- Inspections
- Payments
---
