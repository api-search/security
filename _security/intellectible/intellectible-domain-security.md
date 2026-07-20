---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: intellectible.com
  spf: true
hosts:
- cert_expires: Sep 29 15:10:53 2026 GMT
  host: intellectible.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 10 16:12:31 2026 GMT
  host: docs.intellectible.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 16 19:05:10 2026 GMT
  host: app.intellectible.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Intellectible Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intellectible, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Intellectible
provider_slug: intellectible
slug: intellectible-domain-security
source_filename: intellectible-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intellectible.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 15:10:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.intellectible.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 16:12:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: app.intellectible.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 19:05:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: intellectible.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intellectible/refs/heads/main/security/intellectible-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Artificial Intelligence
- Government
- GovCon
- Proposals
- CRM
- Workflow Automation
- Pricing
- Knowledge Management
- Enterprise Software
- Professional Services
---
