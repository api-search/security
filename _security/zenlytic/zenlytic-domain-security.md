---
api_specs:
- filename: zenlytic-embed-openapi.yml
  format: yaml
  label: Zenlytic Signed Embedding API
  slug: zenlytic-signed-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenlytic/refs/heads/main/openapi/zenlytic-embed-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zenlytic.com
  spf: true
hosts:
- cert_expires: Oct 10 09:03:45 2026 GMT
  host: www.zenlytic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenlytic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenlytic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zenlytic
provider_slug: zenlytic
slug: zenlytic-domain-security
source_filename: zenlytic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zenlytic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 09:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zenlytic.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenlytic/refs/heads/main/security/zenlytic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- Business Intelligence
- Analytics
- Artificial Intelligence
- Data
- Embedded Analytics
- MCP
---
