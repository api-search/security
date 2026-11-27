---
api_specs:
- filename: hamburg-de-access-data-api-openapi.yml
  format: yaml
  label: Freie und Hansestadt Hamburg Access data API
  slug: hamburg-de-access-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hamburg-de/openapi/hamburg-de-access-data-api-openapi.yml
- filename: hamburg-de-capabilities-api-openapi.yml
  format: yaml
  label: Freie und Hansestadt Hamburg Capabilities API
  slug: hamburg-de-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hamburg-de/openapi/hamburg-de-capabilities-api-openapi.yml
- filename: hamburg-de-discover-data-collections-api-openapi.yml
  format: yaml
  label: Freie und Hansestadt Hamburg Discover data collections API
  slug: hamburg-de-discover-data-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hamburg-de/openapi/hamburg-de-discover-data-collections-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "d-trust.net"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:itservices@team.hamburg.de"
  - 0 issue "certum.pl"
  - 0 issue "starfieldtech.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hamburg.de
  spf: true
hosts:
- cert_expires: Mar 10 05:04:27 2027 GMT
  host: api.hamburg.de
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Freie und Hansestadt Hamburg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freie und Hansestadt Hamburg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Freie und Hansestadt Hamburg
provider_slug: hamburg-de
slug: hamburg-de-domain-security
source_filename: hamburg-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.hamburg.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 10 05:04:27 2027 GMT\n  hsts: false\ndomains:\n- domain: hamburg.de\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"d-trust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:itservices@team.hamburg.de\"\n  - 0 issue \"certum.pl\"\n  - 0 issue \"starfieldtech.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hamburg-de/security/hamburg-de-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Government
- Open Data
- Geospatial
- OGC API Features
- Smart City
- Germany
- Urban Data Platform
---
