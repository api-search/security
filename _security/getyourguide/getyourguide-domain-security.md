---
api_specs:
- filename: getyourguide-bookings-api-openapi.yml
  format: yaml
  label: GetYourGuide Bookings API
  slug: getyourguide-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/openapi/getyourguide-bookings-api-openapi.yml
- filename: getyourguide-carts-api-openapi.yml
  format: yaml
  label: GetYourGuide Carts API
  slug: getyourguide-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/openapi/getyourguide-carts-api-openapi.yml
- filename: getyourguide-categories-api-openapi.yml
  format: yaml
  label: GetYourGuide Categories API
  slug: getyourguide-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/openapi/getyourguide-categories-api-openapi.yml
- filename: getyourguide-configuration-api-openapi.yml
  format: yaml
  label: GetYourGuide Configuration API
  slug: getyourguide-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/openapi/getyourguide-configuration-api-openapi.yml
- filename: getyourguide-options-api-openapi.yml
  format: yaml
  label: GetYourGuide Options API
  slug: getyourguide-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/openapi/getyourguide-options-api-openapi.yml
- filename: getyourguide-reviews-api-openapi.yml
  format: yaml
  label: GetYourGuide Reviews API
  slug: getyourguide-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/openapi/getyourguide-reviews-api-openapi.yml
- filename: getyourguide-suppliers-api-openapi.yml
  format: yaml
  label: GetYourGuide Suppliers API
  slug: getyourguide-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/openapi/getyourguide-suppliers-api-openapi.yml
- filename: getyourguide-tours-api-openapi.yml
  format: yaml
  label: GetYourGuide Tours API
  slug: getyourguide-tours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/openapi/getyourguide-tours-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa-iodef@getyourguide.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getyourguide.com
  spf: true
- caa:
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:caa-iodef@getyourguide.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: gygtest.net
  spf: false
hosts:
- cert_expires: Sep 22 10:39:43 2026 GMT
  host: code.getyourguide.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 10:27:19 2026 GMT
  host: api.getyourguide.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 11:49:09 2026 GMT
  host: api.gygtest.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getyourguide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetYourGuide, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GetYourGuide
provider_slug: getyourguide
slug: getyourguide-domain-security
source_filename: getyourguide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: code.getyourguide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:39:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getyourguide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:27:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gygtest.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:49:09 2026 GMT\n  hsts: null\ndomains:\n- domain: getyourguide.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa-iodef@getyourguide.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gygtest.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:caa-iodef@getyourguide.com\"\n  - 0 issue\
  \ \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getyourguide/refs/heads/main/security/getyourguide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Tourism
- Tours and Activities
- Marketplace
- Booking
- Experiences
- Affiliate
- Partner API
- Ecommerce
---
