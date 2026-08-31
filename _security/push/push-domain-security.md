---
api_specs:
- filename: push-account-api-openapi.yml
  format: yaml
  label: Push Account API
  slug: push-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-account-api-openapi.yml
- filename: push-audience-list-api-openapi.yml
  format: yaml
  label: Push Audience List API
  slug: push-audience-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-audience-list-api-openapi.yml
- filename: push-campaigns-api-openapi.yml
  format: yaml
  label: Push Campaigns API
  slug: push-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-campaigns-api-openapi.yml
- filename: push-company-api-openapi.yml
  format: yaml
  label: Push Company API
  slug: push-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-company-api-openapi.yml
- filename: push-company-custom-fields-api-openapi.yml
  format: yaml
  label: Push Company custom fields API
  slug: push-company-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-company-custom-fields-api-openapi.yml
- filename: push-contact-api-openapi.yml
  format: yaml
  label: Push Contact API
  slug: push-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-contact-api-openapi.yml
- filename: push-contact-custom-fields-api-openapi.yml
  format: yaml
  label: Push Contact Custom fields API
  slug: push-contact-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-contact-custom-fields-api-openapi.yml
- filename: push-coupon-lists-api-openapi.yml
  format: yaml
  label: Push Coupon lists API
  slug: push-coupon-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-coupon-lists-api-openapi.yml
- filename: push-deliveries-api-openapi.yml
  format: yaml
  label: Push Deliveries API
  slug: push-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-deliveries-api-openapi.yml
- filename: push-hotel-data-api-openapi.yml
  format: yaml
  label: Push Hotel Data API
  slug: push-hotel-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-hotel-data-api-openapi.yml
- filename: push-hotel-data-custom-fields-api-openapi.yml
  format: yaml
  label: Push Hotel Data custom fields API
  slug: push-hotel-data-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-hotel-data-custom-fields-api-openapi.yml
- filename: push-product-api-openapi.yml
  format: yaml
  label: Push Product API
  slug: push-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-product-api-openapi.yml
- filename: push-product-custom-fields-api-openapi.yml
  format: yaml
  label: Push Product custom fields API
  slug: push-product-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-product-custom-fields-api-openapi.yml
- filename: push-purchase-api-openapi.yml
  format: yaml
  label: Push Purchase API
  slug: push-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-purchase-api-openapi.yml
- filename: push-sync-data-api-openapi.yml
  format: yaml
  label: Push Sync Data API
  slug: push-sync-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-sync-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pushtech.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cendyncrm.com
  spf: false
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: pushtech.com
  hsts: false
  https: true
  role: legacy marketing site
  tls_version: TLSv1.3
- cert_expires: Nov  1 18:29:53 2026 GMT
  host: developers.cendyncrm.com
  hsts: false
  https: true
  role: developer portal / API reference
  tls_version: TLSv1.3
- cert_expires: Oct 31 10:26:20 2026 GMT
  host: api.eu.cendyncrm.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  http_version: HTTP/2
  https: true
  role: API base URL (EU data center)
  tls_version: TLSv1.3
- host: api.us.cendyncrm.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  http_version: HTTP/2
  https: true
  role: API base URL (US data center)
- host: www.cendyn.com
  http_status: 403
  https: true
  note: Cloudflare bot challenge on every request, including with a browser User-Agent. TLS and header posture could not be assessed. This is an unprobeable host, not a security finding.
  reachable: false
  role: parent-company marketing site
kind: domain-security
layout: security
method: probed
name: Push Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Push, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Push
provider_slug: push
slug: push-domain-security
source_filename: push-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI servers[] hosts\nhosts:\n- host: pushtech.com\n  role: legacy marketing site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\n- host: developers.cendyncrm.com\n  role: developer portal / API reference\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 18:29:53 2026 GMT\n  hsts: false\n- host: api.eu.cendyncrm.com\n  role: API base URL (EU data center)\n  https: true\n  http_version: HTTP/2\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 10:26:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n- host: api.us.cendyncrm.com\n  role: API base URL (US data center)\n  https: true\n  http_version: HTTP/2\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n- host: www.cendyn.com\n  role: parent-company marketing site\n  https: true\n  reachable: false\n  http_status: 403\n\
  \  note: >-\n    Cloudflare bot challenge on every request, including with a browser User-Agent. TLS and header\n    posture could not be assessed. This is an unprobeable host, not a security finding.\ndomains:\n- domain: pushtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cendyncrm.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\nfindings:\n- HSTS is enabled on both API hosts with a two-year max-age and includeSubDomains, but is absent on the developer portal and the legacy marketing site.\n- No CAA record on either registrable domain — any CA may issue for them.\n- No DNSSEC on either registrable domain.\n- 'cendyncrm.com — the domain that serves the live API and the developer portal — publishes no SPF record and a DMARC policy of p=none, so it is neither protected against spoofing nor enforcing. Notable for a platform whose product is sending email on customers'' behalf.'\n- 'The retired pushtech.com\
  \ domain has the stronger email posture of the two (SPF present, DMARC p=quarantine); the active brand''s domain has the weaker one.'\ndead_hosts:\n- {host: developers.pushtech.com, dns: NXDOMAIN, note: 'former developer portal; retired without a redirect'}\n- {host: help.pushtech.com, dns: NXDOMAIN, note: 'former help centre'}\n- {host: www.cendyncrm.com, dns: 'no A record', note: 'the sign-in and manager links published in the live developer portal point here and are broken'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/security/push-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Customer Data Platform
- Marketing Automation
- Hospitality
- Hotels
- Guest Experience
- Email
- SMS
- Push Notifications
- Webhook
- Segmentation
---
