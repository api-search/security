---
api_specs:
- filename: kanmon-openapi-original.yml
  format: yaml
  label: Kanmon Public V2 API
  slug: kanmon-public-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kanmonhq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kanmon.com
  spf: true
hosts:
- cert_expires: Sep  1 05:23:27 2026 GMT
  host: www.kanmonhq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 22:43:09 2026 GMT
  host: api.kanmon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 18:23:29 2026 GMT
  host: api.kanmon.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kanmon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kanmon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kanmon
provider_slug: kanmon
slug: kanmon-domain-security
source_filename: kanmon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kanmonhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 05:23:27 2026 GMT\n  hsts: null\n- host: api.kanmon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:43:09 2026 GMT\n  hsts: null\n- host: api.kanmon.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 18:23:29 2026 GMT\n  hsts: null\ndomains:\n- domain: kanmonhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kanmon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/security/kanmon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Embedded Finance
- Embedded Lending
- Lending
- Working Capital
- Invoice Financing
- API
---
