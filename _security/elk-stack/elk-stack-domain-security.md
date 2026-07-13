---
api_specs:
- filename: elasticsearch-serverless-openapi.json
  format: json
  label: Elasticsearch API
  slug: elasticsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/elastic/elasticsearch-specification/main/output/openapi/elasticsearch-serverless-openapi.json
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
name: Elk Stack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elastic Stack (ELK Stack), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elastic Stack (ELK Stack)
provider_slug: elk-stack
slug: elk-stack-domain-security
source_filename: elk-stack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elastic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 21:06:03 2026 GMT\n  hsts: false\ndomains:\n- domain: elastic.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elk-stack/refs/heads/main/security/elk-stack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Logging
- Monitoring
- Observability
- Search
---
