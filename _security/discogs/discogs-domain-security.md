---
api_specs:
- filename: discogs-database-api-openapi.yml
  format: yaml
  label: Discogs Database API
  slug: discogs-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/openapi/discogs-database-api-openapi.yml
- filename: discogs-image-api-openapi.yml
  format: yaml
  label: Discogs Image API
  slug: discogs-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/openapi/discogs-image-api-openapi.yml
- filename: discogs-inventory-management-api-openapi.yml
  format: yaml
  label: Discogs Inventory Management API
  slug: discogs-inventory-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/openapi/discogs-inventory-management-api-openapi.yml
- filename: discogs-marketplace-api-openapi.yml
  format: yaml
  label: Discogs Marketplace API
  slug: discogs-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/openapi/discogs-marketplace-api-openapi.yml
- filename: discogs-user-collection-api-openapi.yml
  format: yaml
  label: Discogs User Collection API
  slug: discogs-user-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/openapi/discogs-user-collection-api-openapi.yml
- filename: discogs-user-identity-api-openapi.yml
  format: yaml
  label: Discogs User Identity API
  slug: discogs-user-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/openapi/discogs-user-identity-api-openapi.yml
- filename: discogs-user-lists-api-openapi.yml
  format: yaml
  label: Discogs User Lists API
  slug: discogs-user-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/openapi/discogs-user-lists-api-openapi.yml
- filename: discogs-user-wantlist-api-openapi.yml
  format: yaml
  label: Discogs User Wantlist API
  slug: discogs-user-wantlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/openapi/discogs-user-wantlist-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: discogs.com
  spf: true
hosts:
- cert_expires: Aug 28 19:31:07 2026 GMT
  host: www.discogs.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 19:31:07 2026 GMT
  host: api.discogs.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Discogs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Discogs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Discogs
provider_slug: discogs
slug: discogs-domain-security
source_filename: discogs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.discogs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:31:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.discogs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:31:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: discogs.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/security/discogs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Marketplace
- Catalog
- Community
- Vinyl
- Public APIs
---
