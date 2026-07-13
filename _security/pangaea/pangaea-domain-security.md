---
api_specs:
- filename: _search
  format: yaml
  label: PANGAEA Elasticsearch Search API
  slug: pangaea-elasticsearch-search-api
  spec_type: OpenAPI
  url: https://ws.pangaea.de/es/pangaea/panmd/_search
- filename: provider
  format: yaml
  label: PANGAEA OAI-PMH Metadata Harvesting API
  slug: pangaea-oai-pmh-metadata-harvesting-api
  spec_type: OpenAPI
  url: https://ws.pangaea.de/oai/provider?verb=Identify
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.dfn.de"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pangaea.de
  spf: true
hosts:
- cert_expires: Sep  4 05:40:36 2026 GMT
  host: wiki.pangaea.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 05:40:36 2026 GMT
  host: ws.pangaea.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 05:40:36 2026 GMT
  host: www.pangaea.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pangaea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PANGAEA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PANGAEA
provider_slug: pangaea
slug: pangaea-domain-security
source_filename: pangaea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wiki.pangaea.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 05:40:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ws.pangaea.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 05:40:36 2026 GMT\n  hsts: false\n- host: www.pangaea.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 05:40:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pangaea.de\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.dfn.de\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pangaea/refs/heads/main/security/pangaea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Earth Science
- Ocean Data
- Climate Records
- Environmental Science
- Geoscience
- Open Data
- Scientific Data
---
