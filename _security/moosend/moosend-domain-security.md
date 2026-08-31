---
api_specs:
- filename: moosend-campaigns-api-openapi.yml
  format: yaml
  label: Moosend Campaigns API
  slug: moosend-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moosend/refs/heads/main/openapi/moosend-campaigns-api-openapi.yml
- filename: moosend-mailing-lists-api-openapi.yml
  format: yaml
  label: Moosend Mailing Lists API
  slug: moosend-mailing-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moosend/refs/heads/main/openapi/moosend-mailing-lists-api-openapi.yml
- filename: moosend-segments-api-openapi.yml
  format: yaml
  label: Moosend Segments API
  slug: moosend-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moosend/refs/heads/main/openapi/moosend-segments-api-openapi.yml
- filename: moosend-subscribers-api-openapi.yml
  format: yaml
  label: Moosend Subscribers API
  slug: moosend-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moosend/refs/heads/main/openapi/moosend-subscribers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moosend.com
  spf: true
hosts:
- cert_expires: Apr  6 16:03:03 2027 GMT
  host: moosend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 18:13:52 2026 GMT
  host: api.moosend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moosend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moosend, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Moosend
provider_slug: moosend
slug: moosend-domain-security
source_filename: moosend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moosend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 16:03:03 2027 GMT\n  hsts: false\n- host: api.moosend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 18:13:52 2026 GMT\n  hsts: null\ndomains:\n- domain: moosend.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moosend/refs/heads/main/security/moosend-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Marketing
- Marketing Automation
- Campaigns
- Mailing Lists
- Subscribers
- Transactional Email
- SMTP
- Segmentation
- Analytics
- Email
- Newsletters
- Landing Pages
- Website Tracking
- Marketing
---
