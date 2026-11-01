---
api_specs:
- filename: appcheck-ng-openapi-generated.yml
  format: yaml
  label: APPCHECK API
  slug: appcheck-ng-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appcheck-ng/openapi/_ae-authored/appcheck-ng-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appcheck-ng.com
  spf: true
hosts:
- cert_expires: Apr 22 19:39:28 2027 GMT
  host: appcheck-ng.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Appcheck Ng Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APPCHECK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: APPCHECK
provider_slug: appcheck-ng
slug: appcheck-ng-domain-security
source_filename: appcheck-ng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appcheck-ng.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 22 19:39:28 2027 GMT\n  hsts: false\ndomains:\n- domain: appcheck-ng.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/appcheck-ng/security/appcheck-ng-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web Application Scanning
- API Security
- Infrastructure Scanning
- CMS Security
- Single Page Application Scanning
- Automated Penetration Testing
---
