---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: definityfinancial.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: economical.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sonnet.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: petsecure.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: definity.com
  note: SPF record names the third-party services fronting Definity's mail and broker estate, including spf.acturis.com (Acturis broker management system), docebosaas.com (broker LMS), service-now.com, salesforce.com, sendgrid.net and spf.protection.outlook.com.
  spf: true
hosts:
- cert_expires: Sep 19 14:22:17 2026 GMT
  host: www.definityfinancial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: www.economical.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: www.sonnet.ca
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: www.petsecure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.definity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Partner/production gateway. Imperva-fronted; HTTP 404 with empty body to all anonymous paths.
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: broker.economical.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Docebo SaaS learning management system for broker training (CNAME economical.docebosaas.com).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Definity Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Definity Financial, probed live across 6 host(s) and 5 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Definity Financial
provider_slug: definity-financial
slug: definity-financial-domain-security
source_filename: definity-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.definityfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 14:22:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.economical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.sonnet.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: www.petsecure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.definity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Partner/production gateway. Imperva-fronted; HTTP 404 with empty body to all anonymous paths.\n- host: broker.economical.com\n  https:\
  \ true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Docebo SaaS learning management system for broker training (CNAME economical.docebosaas.com).\ndomains:\n- domain: definityfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: economical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sonnet.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: petsecure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: definity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    SPF record names the third-party services fronting Definity's mail and broker estate,\n    including spf.acturis.com (Acturis broker management system), docebosaas.com (broker\n    LMS), service-now.com,\
  \ salesforce.com, sendgrid.net and spf.protection.outlook.com.\nfindings:\n- No domain in the estate publishes DNSSEC.\n- No domain in the estate publishes a CAA record.\n- All five domains publish SPF with a -all hard fail.\n- >-\n  DMARC is published everywhere but four of five domains sit at p=none (monitor only);\n  only petsecure.com enforces at p=quarantine. No domain reaches p=reject.\n- All six probed hosts serve TLS 1.3 with HSTS; only broker.economical.com sets includeSubDomains.\nextended_probe:\n  method: probed\n  source: >-\n    dig against 8.8.8.8 plus openssl s_client and HEAD requests, run 2026-07-25 to cover the\n    petsecure.com, api.definity.com, broker.economical.com and definity.com surfaces that the\n    apis.yml-driven pass did not reach.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/definity-financial/refs/heads/main/security/definity-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Property and Casualty
- Carrier
- Underwriting
- Claims
- Broker
- Pet Insurance
- Direct to Consumer
- Partner Gated
- CSIO
- Insurtech
---
