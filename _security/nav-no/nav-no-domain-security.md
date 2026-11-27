---
api_specs:
- filename: nav-no-feed-api-openapi.yml
  format: yaml
  label: NAV (Norwegian Labour and Welfare Administration) Feed API
  slug: nav-no-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nav-no/openapi/nav-no-feed-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "buypass.com"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:hostmaster@nav.no"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nav.no
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: www.nav.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NAV (Norwegian Labour and Welfare Administration) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NAV (Norwegian Labour and Welfare Administration), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NAV (Norwegian Labour and Welfare Administration)
provider_slug: nav-no
slug: nav-no-domain-security
source_filename: nav-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nav.no\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nav.no\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"buypass.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:hostmaster@nav.no\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nav-no/security/nav-no-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Employment
- Job Vacancies
- Public Sector
- Norway
- Welfare
---
