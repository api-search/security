---
api_specs:
- filename: open-brewery-db-breweries-api-openapi.yml
  format: yaml
  label: Open Brewery DB Breweries API
  slug: open-brewery-db-breweries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-brewery-db/refs/heads/main/openapi/open-brewery-db-breweries-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbrewerydb.org
  spf: true
hosts:
- cert_expires: Aug 30 10:48:48 2026 GMT
  host: www.openbrewerydb.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 21:31:09 2026 GMT
  host: api.openbrewerydb.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Brewery Db Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Brewery DB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Open Brewery DB
provider_slug: open-brewery-db
slug: open-brewery-db-domain-security
source_filename: open-brewery-db-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openbrewerydb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 10:48:48 2026 GMT\n  hsts: false\n- host: api.openbrewerydb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 21:31:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openbrewerydb.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-brewery-db/refs/heads/main/security/open-brewery-db-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Beer
- Bottle Shops
- Brew Pubs
- Breweries
- Cider
---
