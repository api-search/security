---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: soona.co
  spf: true
  spf_record: v=spf1 a mx include:_spf.google.com include:sendgrid.net include:23618366.spf03.hubspotemail.net -all
- caa: []
  dmarc: false
  dnssec: false
  domain: mokker.ai
  finding: mokker.ai accepts mail (Google Workspace MX) but publishes neither an SPF record nor a DMARC record, so the domain is unprotected against spoofing. soona.co by contrast publishes SPF with a -all hard fail, though its DMARC policy is p=none (monitor only, no enforcement).
  mx: true
  spf: false
hosts:
- cert_expires: Oct  3 02:31:29 2026 GMT
  host: soona.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: book.soona.co
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  server: Heroku
  tls_version: TLSv1.3
- host: mokker.ai
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  server: Framer
  tls_version: TLSv1.3
- host: app.mokker.ai
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 63072000
  http_status: 307
  https: true
  server: Vercel
  tls_version: TLSv1.3
- detail: api.mokker.ai is a CNAME to dualstack.mokker-us-west-2-prod-api-lb-1256808001.us-west-2.elb.amazonaws.com, which answers NXDOMAIN — the AWS load balancer it points at no longer exists. This is the exact host advertised as the API base on https://mokker.ai/api. A CNAME left pointing at a deleted cloud resource is a standing subdomain-takeover exposure as well as a dead API endpoint.
  finding: dangling-cname
  host: api.mokker.ai
  https: null
  resolves: false
kind: domain-security
layout: security
method: probed
name: Soona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for soona, probed live across 5 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: soona
provider_slug: soona
slug: soona-domain-security
source_filename: soona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the soona-controlled application and mokker.ai hosts\nnote: >-\n  The soona.co row was written by 0-working/probe-domain-security.py; the book.soona.co,\n  mokker.ai, app.mokker.ai and api.mokker.ai rows were probed by hand in the same pass\n  (curl HEAD + openssl s_client + dig), because the script only reads hosts named in\n  apis.yml and soona names no APIs. mokker.ai is a soona property, acquired with Zerolens\n  GmbH in March 2024.\nhosts:\n- host: soona.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:31:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: book.soona.co\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  server: Heroku\n- host: mokker.ai\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  server: Framer\n\
  - host: app.mokker.ai\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: false\n  server: Vercel\n  http_status: 307\n- host: api.mokker.ai\n  https: null\n  resolves: false\n  finding: dangling-cname\n  detail: >-\n    api.mokker.ai is a CNAME to\n    dualstack.mokker-us-west-2-prod-api-lb-1256808001.us-west-2.elb.amazonaws.com, which\n    answers NXDOMAIN — the AWS load balancer it points at no longer exists. This is the\n    exact host advertised as the API base on https://mokker.ai/api. A CNAME left pointing\n    at a deleted cloud resource is a standing subdomain-takeover exposure as well as a dead\n    API endpoint.\ndomains:\n- domain: soona.co\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 a mx include:_spf.google.com include:sendgrid.net include:23618366.spf03.hubspotemail.net -all\n  dmarc: true\n  dmarc_policy: none\n- domain: mokker.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  mx: true\n\
  \  finding: >-\n    mokker.ai accepts mail (Google Workspace MX) but publishes neither an SPF record nor a\n    DMARC record, so the domain is unprotected against spoofing. soona.co by contrast\n    publishes SPF with a -all hard fail, though its DMARC policy is p=none (monitor only,\n    no enforcement).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soona/refs/heads/main/security/soona-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- E-Commerce
- Content
- Photography
- Video
- Creative
- Digital Asset Management
- Artificial Intelligence
- Marketing
---
