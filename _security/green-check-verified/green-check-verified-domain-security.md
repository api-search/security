---
api_specs:
- filename: green-check-verified-access-openapi.yaml
  format: yaml
  label: Green Check Access
  slug: green-check-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-check-verified/refs/heads/main/openapi/green-check-verified-access-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: greencheckverified.com
  spf: true
hosts:
- cert_expires: Oct 22 15:15:19 2026 GMT
  host: greencheckverified.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 06:05:32 2026 GMT
  host: developer.greencheckverified.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: prod-api.greencheckverified.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Check Verified Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Check Verified, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Green Check Verified
provider_slug: green-check-verified
slug: green-check-verified-domain-security
source_filename: green-check-verified-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greencheckverified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 15:15:19 2026 GMT\n  hsts: false\n- host: developer.greencheckverified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 06:05:32 2026 GMT\n  hsts: false\n- host: prod-api.greencheckverified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: greencheckverified.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-check-verified/refs/heads/main/security/green-check-verified-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cannabis
- Compliance
- Banking
- Financial Services
- BSA/AML
- Regulatory Technology
- Point of Sale
- Onboarding
- Due Diligence
- Know Your Customer
- Data Aggregation
---
