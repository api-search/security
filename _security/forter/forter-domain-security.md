---
api_specs:
- filename: forter-openapi.yml
  format: yaml
  label: Forter Order Decision API
  slug: forter-order-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
- filename: forter-openapi.yml
  format: yaml
  label: Forter Account Protection API
  slug: forter-account-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
- filename: forter-openapi.yml
  format: yaml
  label: Forter Chargeback and Compensation API
  slug: forter-chargeback-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
- filename: forter-openapi.yml
  format: yaml
  label: Forter Data Privacy API
  slug: forter-data-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/openapi/forter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: forter.com
  spf: true
  spf_record: v=spf1 include:95bc97.workshop-spf.net include:_netblocks.google.com include:_netblocks2.google.com include:_netblocks3.google.com include:2776164.spf01.hubspotemail.net include:_spf.atlassian.net include:_spf.salesforce.com ~all
hosts:
- cert_expires: Sep 13 18:55:22 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: forter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 11:58:39 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: docs.forter.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  cert_issuer: Amazon (Amazon RSA 2048 M04)
  host: portal.forter.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.forter.secure.com
  https: unknown
  note: The bare host api.forter.secure.com does not resolve. The Forter API is served on a per-tenant host - requests go to https://{siteId}.api.forter.secure.com - so the generic host has no public DNS record and could not be probed directly.
kind: domain-security
layout: security
method: probed
name: Forter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forter, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Forter
provider_slug: forter
slug: forter-domain-security
source_filename: forter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:55:22 2026 GMT\n  cert_issuer: Google Trust Services (WE1)\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.forter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 11:58:39 2026 GMT\n  cert_issuer: Google Trust Services (WE1)\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: portal.forter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  cert_issuer: Amazon (Amazon RSA 2048 M04)\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: api.forter.secure.com\n  https: unknown\n  note: >-\n    The bare host api.forter.secure.com does not resolve. The Forter API is\n    served on a per-tenant host - requests go to https://{siteId}.api.forter.secure.com -\n    so the generic\
  \ host has no public DNS record and could not be probed\n    directly.\ndomains:\n- domain: forter.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:95bc97.workshop-spf.net include:_netblocks.google.com include:_netblocks2.google.com include:_netblocks3.google.com include:2776164.spf01.hubspotemail.net include:_spf.atlassian.net include:_spf.salesforce.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forter/refs/heads/main/security/forter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Detection
- Fraud Prevention
- Identity
- Trust
- Payments
- Chargebacks
- Account Protection
- E-commerce
- Risk
- Machine Learning
---
