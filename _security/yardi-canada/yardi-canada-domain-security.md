---
api_specs:
- filename: yardi-canada-components-api-openapi.yml
  format: yaml
  label: Yardi Canada Components API
  slug: yardi-canada-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-components-api-openapi.yml
- filename: yardi-canada-incidents-api-openapi.yml
  format: yaml
  label: Yardi Canada Incidents API
  slug: yardi-canada-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-incidents-api-openapi.yml
- filename: yardi-canada-maintenance-api-openapi.yml
  format: yaml
  label: Yardi Canada Maintenance API
  slug: yardi-canada-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-maintenance-api-openapi.yml
- filename: yardi-canada-status-api-openapi.yml
  format: yaml
  label: Yardi Canada Status API
  slug: yardi-canada-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yardibreeze.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yardi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: virtuoso.ai
  note: The virtuoso.ai SPF record includes asp-spf1.yardi.com, asp-spf2.yardi.com and other-spf1.yardi.com, corroborating that virtuoso.ai is operated by Yardi. DMARC is p=none (monitor only) with Proofpoint aggregate/forensic reporting.
  spf: true
hosts:
- cert_expires: Sep 22 15:20:24 2026 GMT
  host: www.yardibreeze.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 02:36:40 2026 GMT
  host: www.yardi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 18:47:30 2026 GMT
  host: resources.yardi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 12:22:38 2026 GMT
  host: status.yardi.com
  hsts: true
  hsts_max_age: 259200
  https: true
  note: Public status API host. HSTS max-age is 259200 (3 days) — two orders of magnitude shorter than the 31536000 the Yardi web properties set, and below the 31536000 required for preload.
  tls_version: TLSv1.3
- cert_expires: Sep 23 04:41:14 2026 GMT
  host: mcp.virtuoso.ai
  hsts: false
  https: true
  note: Yardi Virtuoso MCP server. No Strict-Transport-Security header was observed; the HEAD probe was answered with a Cloudflare 403, so absence is recorded as observed on that response rather than as a confirmed policy.
  tls_version: TLSv1.3
- cert_expires: Sep 22 19:48:45 2026 GMT
  host: virtuoso.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yardi Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yardi Canada, probed live across 6 host(s) and 3 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Yardi Canada
provider_slug: yardi-canada
slug: yardi-canada-domain-security
source_filename: yardi-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yardibreeze.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:20:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.yardi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 02:36:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: resources.yardi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 18:47:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.yardi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:22:38 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n  note: >-\n    Public status API host. HSTS max-age is 259200 (3 days) — two orders of magnitude\n    shorter than the 31536000 the Yardi web properties set, and below the 31536000\n    required for preload.\n- host: mcp.virtuoso.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires:\
  \ Sep 23 04:41:14 2026 GMT\n  hsts: false\n  note: >-\n    Yardi Virtuoso MCP server. No Strict-Transport-Security header was observed; the\n    HEAD probe was answered with a Cloudflare 403, so absence is recorded as observed\n    on that response rather than as a confirmed policy.\n- host: virtuoso.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 19:48:45 2026 GMT\n  hsts: false\ndomains:\n- domain: yardibreeze.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: yardi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: virtuoso.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    The virtuoso.ai SPF record includes asp-spf1.yardi.com, asp-spf2.yardi.com and\n    other-spf1.yardi.com, corroborating that virtuoso.ai is operated by Yardi. DMARC\n    is p=none (monitor only) with Proofpoint aggregate/forensic reporting.\nfindings:\n- No domain in the estate is DNSSEC-signed.\n\
  - No domain publishes a CAA record, so any CA may issue for yardi.com, yardibreeze.ca or virtuoso.ai.\n- yardibreeze.ca — the live Canadian property — publishes no DMARC record at all; yardi.com is at quarantine and virtuoso.ai at none. No domain reaches p=reject.\n- TLS 1.3 everywhere, and HSTS with a one-year max-age on the three web hosts; the MCP host and the marketplace host set no HSTS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/security/yardi-canada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Canada
- Property Management
- Rentals
- Commercial Real Estate
- PropTech
- Multifamily
- Affordable Housing
- Senior Living
- Investment Management
- Tenancy
- Payments
- MCP
- Artificial Intelligence
---
