---
api_specs:
- filename: sertica-web-api-openapi.json
  format: json
  label: SERTICA Web API
  slug: sertica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertica/refs/heads/main/openapi/sertica-web-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sertica.com
  spf: true
hosts:
- cert_expires: Nov  1 06:08:12 2026 GMT
  host: www.sertica.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sertica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SERTICA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SERTICA
provider_slug: sertica
slug: sertica-domain-security
source_filename: sertica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sertica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 06:08:12 2026 GMT\n  hsts: false\ndomains:\n- domain: sertica.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sertica/refs/heads/main/security/sertica-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Maritime
- Shipping
- Fleet Management
- Maintenance
- Procurement
- Asset Management
- Compliance
- Enterprise Software
---
