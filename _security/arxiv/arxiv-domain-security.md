---
api_specs:
- filename: arxiv-query-openapi.yml
  format: yaml
  label: arXiv Query API
  slug: arxiv-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arxiv/refs/heads/main/openapi/arxiv-query-openapi.yml
- filename: arxiv-oaipmh-openapi.yml
  format: yaml
  label: arXiv OAI-PMH API
  slug: arxiv-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arxiv/refs/heads/main/openapi/arxiv-oaipmh-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arxiv.org
  spf: true
hosts:
- cert_expires: Jul 27 05:26:48 2026 GMT
  host: arxiv.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 15:51:33 2026 GMT
  host: info.arxiv.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 27 05:26:48 2026 GMT
  host: export.arxiv.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arxiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for arXiv, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: arXiv
provider_slug: arxiv
slug: arxiv-domain-security
source_filename: arxiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arxiv.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 05:26:48 2026 GMT\n  hsts: false\n- host: info.arxiv.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:51:33 2026 GMT\n  hsts: false\n- host: export.arxiv.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 05:26:48 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: arxiv.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arxiv/refs/heads/main/security/arxiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Science And Math
- Scholarly Publishing
- Preprints
- Open Access
- Research
- Open Source
- Public APIs
---
