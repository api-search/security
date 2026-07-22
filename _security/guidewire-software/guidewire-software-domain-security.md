---
description: ''
domains:
- caa:
  - 0 issue "starfieldtech.com"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: guidewire.com
  spf: true
hosts:
- cert_expires: Oct 15 18:31:48 2026 GMT
  host: www.guidewire.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guidewire Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guidewire Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Guidewire Software
provider_slug: guidewire-software
slug: guidewire-software-domain-security
source_filename: guidewire-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guidewire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:31:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: guidewire.com\n  dnssec: false\n  caa:\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guidewire-software/refs/heads/main/security/guidewire-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Property and Casualty
- Cloud
- Policy Administration
- Claims Management
- Billing
- APIs
- Integration
---
