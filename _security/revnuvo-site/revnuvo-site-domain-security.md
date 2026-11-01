---
api_specs:
- filename: revnuvo-site-domain-api-openapi.yml
  format: yaml
  label: revnuvo-site Domain API
  slug: revnuvo-site-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/revnuvo-site/openapi/revnuvo-site-domain-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: revnuvo.site
  spf: true
hosts:
- cert_expires: Jan 26 11:47:07 2027 GMT
  host: revnuvo.site
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Revnuvo Site Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for revnuvo-site, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: revnuvo-site
provider_slug: revnuvo-site
slug: revnuvo-site-domain-security
source_filename: revnuvo-site-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revnuvo.site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 11:47:07 2027 GMT\n  hsts: false\ndomains:\n- domain: revnuvo.site\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/revnuvo-site/security/revnuvo-site-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Revenue
- SaaS
- Billing
- Finance
---
