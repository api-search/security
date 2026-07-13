---
api_specs:
- filename: client
  format: yaml
  label: Glean Client API
  slug: glean-client-api
  spec_type: OpenAPI
  url: https://developers.glean.com/oas/client
- filename: indexing
  format: yaml
  label: Glean Indexing API
  slug: glean-indexing-api
  spec_type: OpenAPI
  url: https://developers.glean.com/oas/indexing
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: glean.com
  spf: true
hosts:
- cert_expires: Sep 11 01:35:43 2026 GMT
  host: www.glean.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 01:28:53 2026 GMT
  host: developers.glean.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glean, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Glean
provider_slug: glean
slug: glean-domain-security
source_filename: glean-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.glean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:35:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.glean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 01:28:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: glean.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glean/refs/heads/main/security/glean-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agents
- AI
- Answers
- Chat
- Connectors
- Enterprise Search
- Generative AI
- Indexing
- Knowledge
- RAG
- Search
- Work Assistant
---
