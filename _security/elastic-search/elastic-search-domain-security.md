---
api_specs:
- filename: elasticsearch-specification
  format: yaml
  label: Elasticsearch REST API
  slug: elasticsearch-rest-api
  spec_type: OpenAPI
  url: https://github.com/elastic/elasticsearch-specification
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elastic.co
  spf: true
hosts:
- cert_expires: Dec 12 21:06:03 2026 GMT
  host: www.elastic.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elastic Search Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elasticsearch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elasticsearch
provider_slug: elastic-search
slug: elastic-search-domain-security
source_filename: elastic-search-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elastic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 21:06:03 2026 GMT\n  hsts: false\ndomains:\n- domain: elastic.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-search/refs/heads/main/security/elastic-search-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Database
- Distributed Systems
- Full-Text Search
- NoSQL
- Search
---
