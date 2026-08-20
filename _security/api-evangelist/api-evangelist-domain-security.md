---
api_specs:
- filename: apievangelist-v1-openapi.yml
  format: yaml
  label: API Evangelist Network API
  slug: api-evangelist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist/refs/heads/main/openapi/apievangelist-v1-openapi.yml
- filename: apievangelist-governance-openapi.json
  format: json
  label: API Evangelist Governance & Discovery API
  slug: api-evangelist-governance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist/refs/heads/main/openapi/apievangelist-governance-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apievangelist.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: spotlight-rules.com
  spf: false
hosts:
- cert_expires: Oct  9 01:06:24 2026 GMT
  host: apievangelist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 01:06:24 2026 GMT
  host: developer.apievangelist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: api.apievangelist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: mcp.apievangelist.com
  hsts: null
  hsts_note: HEAD / returns 405 (JSON-RPC only), so no HSTS header could be read
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 05:19:41 2026 GMT
  host: spotlight-rules.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api Evangelist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Evangelist, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: API Evangelist
provider_slug: api-evangelist
slug: api-evangelist-domain-security
source_filename: api-evangelist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the apievangelist.com hosts and spotlight-rules.com\nnote: >-\n  Probed by hand rather than by 0-working/probe-domain-security.py: that script's shared\n  provider_hosts() helper EXCLUDES apievangelist.com, because for every other repo in the network\n  an apievangelist.com URL is our own annotation rather than the provider's host. On this one repo\n  apievangelist.com IS the provider, so the automated pass had captured only spotlight-rules.com.\nhosts:\n- host: apievangelist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:06:24 2026 GMT\n  hsts: false\n- host: developer.apievangelist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:06:24 2026 GMT\n  hsts: false\n- host: api.apievangelist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\n- host: mcp.apievangelist.com\n  https: true\n  tls_version: TLSv1.3\n\
  \  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\n  hsts_note: HEAD / returns 405 (JSON-RPC only), so no HSTS header could be read\n- host: spotlight-rules.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:19:41 2026 GMT\n  hsts: false\ndomains:\n- domain: apievangelist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: spotlight-rules.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\ngaps:\n- No HSTS on any host.\n- No CAA records on either domain.\n- No DNSSEC on either domain.\n- SPF is present on apievangelist.com but no DMARC record exists, so SPF failures have no policy.\n- spotlight-rules.com has neither SPF nor DMARC.\nx-evidence:\n  checked: '2026-08-10'\n  method: TLS handshake + HTTP HEAD for HSTS; dig +short for DNSKEY, CAA, TXT and _dmarc TXT\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist/refs/heads/main/security/api-evangelist-domain-security.yml
summary_line: TLSv1.3
tags:
- API Evangelist
- Developer Portal
- API Research
- API Governance
- API Discovery
- MCP
- Agents
- API Standards
- API Vocabulary
---
