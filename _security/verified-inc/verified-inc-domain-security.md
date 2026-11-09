---
api_specs:
- filename: verified-inc-openapi-generated.yml
  format: yaml
  label: Verified API
  slug: verified-inc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verified-inc/openapi/_ae-authored/verified-inc-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: verified.inc
  spf: true
hosts:
- cert_expires: Jan 21 14:20:29 2027 GMT
  host: verified.inc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Verified Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verified, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Verified
provider_slug: verified-inc
slug: verified-inc-domain-security
source_filename: verified-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verified.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 14:20:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verified.inc\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/verified-inc/security/verified-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Identity Verification
- Onboarding
- Phone Verification
- KYC
- Autofill
- Health Insurance
- Fintech
---
