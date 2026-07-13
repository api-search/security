---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: DataCite REST API
  slug: datacite-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/datacite/lupo/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: DataCite MDS API
  slug: datacite-mds-api
  spec_type: OpenAPI
  url: https://github.com/datacite/sashimi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: DataCite Usage Reports API
  slug: datacite-usage-reports-api
  spec_type: OpenAPI
  url: https://github.com/datacite/sashimi/blob/master/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datacite.org
  spf: true
hosts:
- cert_expires: Sep 14 00:27:38 2026 GMT
  host: datacite.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:46:16 2026 GMT
  host: support.datacite.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.datacite.org
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Datacite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataCite, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DataCite
provider_slug: datacite
slug: datacite-domain-security
source_filename: datacite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datacite.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 00:27:38 2026 GMT\n  hsts: false\n- host: support.datacite.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:46:16 2026 GMT\n  hsts: null\n- host: api.datacite.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: datacite.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/security/datacite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- DOI
- Persistent Identifiers
- Scholarly Metadata
- Research Data
- Open Science
- Linked Data
---
