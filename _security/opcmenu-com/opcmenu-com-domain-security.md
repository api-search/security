---
api_specs:
- filename: opcmenu-com-default-api-openapi.yml
  format: yaml
  label: 独行录 人才 API
  slug: opcmenu-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opcmenu-com/openapi/opcmenu-com-default-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opcmenu.com
  spf: true
hosts:
- cert_expires: Dec 22 04:13:59 2026 GMT
  host: opcmenu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 独行录 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 独行录, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 独行录
provider_slug: opcmenu-com
slug: opcmenu-com-domain-security
source_filename: opcmenu-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opcmenu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 04:13:59 2026 GMT\n  hsts: false\ndomains:\n- domain: opcmenu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/opcmenu-com/security/opcmenu-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
