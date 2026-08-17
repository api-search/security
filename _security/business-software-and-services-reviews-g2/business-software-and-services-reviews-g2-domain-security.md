---
api_specs:
- filename: business-software-and-services-reviews-g2-v2-openapi.yml
  format: yaml
  label: G2 API V2
  slug: g2-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/openapi/business-software-and-services-reviews-g2-v2-openapi.yml
- filename: business-software-and-services-reviews-g2-v2-openapi.yml
  format: yaml
  label: G2 Buyer Intent Data API
  slug: g2-buyer-intent-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/openapi/business-software-and-services-reviews-g2-v2-openapi.yml
- filename: business-software-and-services-reviews-g2-data-solutions-openapi.yml
  format: yaml
  label: G2 Data Solutions API
  slug: g2-data-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: g2.com
  spf: true
hosts:
- cert_expires: Oct 28 03:10:18 2026 GMT
  host: www.g2.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 20:58:38 2026 GMT
  host: documentation.g2.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 07:58:14 2026 GMT
  host: data.g2.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Business Software And Services Reviews G2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Business Software and Services Reviews | G2, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Business Software and Services Reviews | G2
provider_slug: business-software-and-services-reviews-g2
slug: business-software-and-services-reviews-g2-domain-security
source_filename: business-software-and-services-reviews-g2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.g2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 03:10:18 2026 GMT\n  hsts: null\n- host: documentation.g2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:58:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.g2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 07:58:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: g2.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/security/business-software-and-services-reviews-g2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- SaaS
- Software Reviews
- Buyer Intent
- Competitive Intelligence
- Market Intelligence
- Marketplace
- MCP
---
