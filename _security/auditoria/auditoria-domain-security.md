---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: auditoria.ai
  spf: true
hosts:
- cert_expires: Sep 15 04:47:17 2026 GMT
  host: www.auditoria.ai
  hsts: true
  hsts_max_age: 604800
  https: true
  role: marketing site
  tls_version: TLSv1.3
- host: app.auditoria.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  role: customer application
- host: auth.auditoria.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: identity provider (Auth0)
- host: docs.auditoria.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: help center (Zendesk)
- host: status.auditoria.ai
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 259200
  https: true
  role: status page (Atlassian Statuspage)
- host: blog.auditoria.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  role: blog
kind: domain-security
layout: security
method: probed
name: Auditoria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auditoria.AI, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Auditoria.AI
provider_slug: auditoria
slug: auditoria-domain-security
source_filename: auditoria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auditoria.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:47:17 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\n  role: marketing site\n- host: app.auditoria.ai\n  https: true\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  role: customer application\n- host: auth.auditoria.ai\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  role: identity provider (Auth0)\n- host: docs.auditoria.ai\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  role: help center (Zendesk)\n- host: status.auditoria.ai\n  https: true\n  hsts: true\n  hsts_max_age: 259200\n  hsts_include_subdomains: false\n  role: status page (Atlassian Statuspage)\n- host: blog.auditoria.ai\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains:\
  \ true\n  hsts_preload: true\n  role: blog\ndomains:\n- domain: auditoria.ai\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auditoria/refs/heads/main/security/auditoria-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Finance
- Accounting
- Accounts Payable
- Accounts Receivable
- Automation
- ERP
- Agents
- SaaS
- Invoicing
- Procurement
---
