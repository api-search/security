---
api_specs:
- filename: sitejabber-business-api-openapi.yml
  format: yaml
  label: SmartCustomer (Sitejabber) Business API
  slug: smartcustomer-sitejabber-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/openapi/sitejabber-business-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smartcustomer.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sitejabber.com
  spf: true
hosts:
- cert_expires: Nov  6 20:01:15 2026 GMT
  host: www.smartcustomer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api.sitejabber.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 20:01:15 2026 GMT
  host: api.smartcustomer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sitejabber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SiteJabber, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SiteJabber
provider_slug: sitejabber
slug: sitejabber-domain-security
source_filename: sitejabber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartcustomer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 20:01:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sitejabber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\n- host: api.smartcustomer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 20:01:15 2026 GMT\n  hsts: false\ndomains:\n- domain: smartcustomer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sitejabber.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitejabber/refs/heads/main/security/sitejabber-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Reviews
- Consumer Reviews
- Product Reviews
- Reputation Management
- Reviews Management
- E-Commerce
- Trust and Safety
- Google Seller Ratings
- Customer Feedback
- Ratings
- Privacy
---
