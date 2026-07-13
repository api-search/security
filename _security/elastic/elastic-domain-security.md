---
api_specs:
- filename: elastic-elasticsearch-openapi.yml
  format: yaml
  label: Elasticsearch REST API
  slug: elasticsearch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-elasticsearch-openapi.yml
- filename: elastic-kibana-openapi.yml
  format: yaml
  label: Kibana API
  slug: kibana
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-kibana-openapi.yml
- filename: elastic-cloud-openapi.yml
  format: yaml
  label: Elastic Cloud API
  slug: elastic-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/openapi/elastic-cloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elastic.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: elastic-cloud.com
  spf: true
hosts:
- cert_expires: Dec 12 21:06:03 2026 GMT
  host: www.elastic.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.elastic-cloud.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Elastic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elastic, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elastic
provider_slug: elastic
slug: elastic-domain-security
source_filename: elastic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elastic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 21:06:03 2026 GMT\n  hsts: false\n- host: api.elastic-cloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: elastic.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: elastic-cloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic/refs/heads/main/security/elastic-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Search
- Analytics
- Observability
- Security
- Visualization
- Cloud
---
