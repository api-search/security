---
api_specs:
- filename: redirectboss-com-analytics-api-openapi.yml
  format: yaml
  label: RedirectBoss Analytics API
  slug: redirectboss-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redirectboss-com/openapi/redirectboss-com-analytics-api-openapi.yml
- filename: redirectboss-com-hosts-api-openapi.yml
  format: yaml
  label: RedirectBoss Hosts API
  slug: redirectboss-com-hosts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redirectboss-com/openapi/redirectboss-com-hosts-api-openapi.yml
- filename: redirectboss-com-redirects-api-openapi.yml
  format: yaml
  label: RedirectBoss Redirects API
  slug: redirectboss-com-redirects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redirectboss-com/openapi/redirectboss-com-redirects-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: redirectboss.com
  spf: true
hosts:
- cert_expires: Apr 19 23:59:59 2027 GMT
  host: redirectboss.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: RedirectBoss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RedirectBoss, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RedirectBoss
provider_slug: redirectboss-com
slug: redirectboss-com-domain-security
source_filename: redirectboss-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redirectboss.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: redirectboss.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/redirectboss-com/security/redirectboss-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Redirects
- Domain Management
- API
- MCP
- SaaS
---
