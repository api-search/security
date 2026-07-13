---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apisjson.org
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apis.guru
  spf: false
hosts:
- cert_expires: Sep 14 08:02:26 2026 GMT
  host: apisjson.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 15:09:58 2026 GMT
  host: apis.guru
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 02:24:31 2026 GMT
  host: api.apis.guru
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knowledge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Knowledge, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: API Knowledge
provider_slug: knowledge
slug: knowledge-domain-security
source_filename: knowledge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apisjson.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:02:26 2026 GMT\n  hsts: false\n- host: apis.guru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:09:58 2026 GMT\n  hsts: false\n- host: api.apis.guru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 02:24:31 2026 GMT\n  hsts: null\ndomains:\n- domain: apisjson.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: apis.guru\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knowledge/refs/heads/main/security/knowledge-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Knowledge
- Knowledge Graphs
- API Discovery
- API Search
- Catalogs
- Indexes
- Registries
- RAG
- Semantic Web
- JSON-LD
- LLMs
- AI Agents
- Topic
---
