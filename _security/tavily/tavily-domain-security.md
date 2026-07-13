---
api_specs:
- filename: tavily-openapi.yml
  format: yaml
  label: Tavily Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tavily/refs/heads/main/openapi/tavily-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tavily.com
  spf: true
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: www.tavily.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 07:22:15 2026 GMT
  host: docs.tavily.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.tavily.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tavily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tavily, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tavily
provider_slug: tavily
slug: tavily-domain-security
source_filename: tavily-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tavily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: false\n- host: docs.tavily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 07:22:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tavily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tavily.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tavily/refs/heads/main/security/tavily-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Web Search
- AI Agents
- LLMs
- Extract
- Crawl
- Sitemap
- Research
- REST
- LangChain
- LlamaIndex
- Real-Time
---
