---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: youraspire.com
  spf: true
hosts:
- cert_expires: Jan 22 17:04:32 2027 GMT
  host: youraspire.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aspire Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aspire (Powered by MindCloud), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aspire (Powered by MindCloud)
provider_slug: aspire-software
slug: aspire-software-domain-security
source_filename: aspire-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: youraspire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 17:04:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: youraspire.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aspire-software/security/aspire-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Field-Service
- Software
- Automation
- Landscaping
---
