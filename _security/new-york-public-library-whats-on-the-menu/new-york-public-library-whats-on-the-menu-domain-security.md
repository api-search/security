---
api_specs:
- filename: new-york-public-library-whats-on-the-menu-openapi-original.yaml
  format: yaml
  label: NYPL What's On The Menu API
  slug: new-york-public-library-whats-on-the-menu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-public-library-whats-on-the-menu/refs/heads/main/openapi/new-york-public-library-whats-on-the-menu-openapi-original.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nypl.org
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: www.nypl.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.menus.nypl.org
  https: false
kind: domain-security
layout: security
method: probed
name: New York Public Library Whats On The Menu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for New York Public Library What''s On The Menu, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: New York Public Library What's On The Menu
provider_slug: new-york-public-library-whats-on-the-menu
slug: new-york-public-library-whats-on-the-menu-domain-security
source_filename: new-york-public-library-whats-on-the-menu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nypl.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.menus.nypl.org\n  https: false\ndomains:\n- domain: nypl.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-york-public-library-whats-on-the-menu/refs/heads/main/security/new-york-public-library-whats-on-the-menu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Libraries
- Menus
- Restaurants
- History
- Open Data
- Food
- Datasets
- Cultural Heritage
---
