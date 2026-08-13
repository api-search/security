---
api_specs:
- filename: disconetwork-partner-api.yml
  format: yaml
  label: Disco Partner Integration API
  slug: disconetwork-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disconetwork/refs/heads/main/openapi/disconetwork-partner-api.yml
- filename: disconetwork-reporting-api-v1.yml
  format: yaml
  label: Disco Reporting API
  slug: disconetwork-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disconetwork/refs/heads/main/openapi/disconetwork-reporting-api-v1.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: disconetwork.com
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: disconetwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: docs.disconetwork.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: partners.disconetwork.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Disconetwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Disconetwork, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Disconetwork
provider_slug: disconetwork
slug: disconetwork-domain-security
source_filename: disconetwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: disconetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.disconetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\n- host: partners.disconetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: disconetwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disconetwork/refs/heads/main/security/disconetwork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce Media
- Retail Media
- Post-Purchase
- Advertising
- Ecommerce
- AdTech
- Marketing
- Analytics
- Reporting
---
