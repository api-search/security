---
api_specs:
- filename: tidb-cloud-api-openapi.yml
  format: yaml
  label: TiDB Cloud API
  slug: tidb-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidb/refs/heads/main/openapi/tidb-cloud-api-openapi.yml
- filename: tidb-cloud-data-service-openapi.yml
  format: yaml
  label: TiDB Cloud Data Service API
  slug: tidb-cloud-data-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidb/refs/heads/main/openapi/tidb-cloud-data-service-openapi.yml
- filename: tidb-cloud-chat2query-openapi.yml
  format: yaml
  label: TiDB Cloud Chat2Query API
  slug: tidb-cloud-chat2query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidb/refs/heads/main/openapi/tidb-cloud-chat2query-openapi.yml
- filename: tidb-http-api-openapi.yml
  format: yaml
  label: TiDB HTTP API
  slug: tidb-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidb/refs/heads/main/openapi/tidb-http-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pingcap.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tidbcloud.com
  spf: true
hosts:
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: docs.pingcap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.tidbcloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: data.tidbcloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tidb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tidb, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: tidb
provider_slug: tidb
slug: tidb-domain-security
source_filename: tidb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.pingcap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: false\n- host: api.tidbcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\n- host: data.tidbcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pingcap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tidbcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidb/refs/heads/main/security/tidb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags: []
---
