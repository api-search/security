---
api_specs:
- filename: amazon-business-openapi-generated.yml
  format: yaml
  label: Amazon Business API
  slug: amazon-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-business/refs/heads/main/openapi/_ae-authored/amazon-business-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: business.amazon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amazon Business Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Business, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Business
provider_slug: amazon-business
slug: amazon-business-domain-security
source_filename: amazon-business-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: business.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-business/refs/heads/main/security/amazon-business-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- B2B
- Procurement
- Marketplace
- BulkPurchasing
---
