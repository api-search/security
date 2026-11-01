---
api_specs:
- filename: recast-software-openapi-generated.yml
  format: yaml
  label: Recast Software API
  slug: recast-software-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recast-software/openapi/_ae-authored/recast-software-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "\"pki.goog; cansignhttpexchanges=yes\""
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: recastsoftware.com
  spf: true
hosts:
- cert_expires: Oct 28 21:41:16 2026 GMT
  host: www.recastsoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Recast Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recast Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Recast Software
provider_slug: recast-software
slug: recast-software-domain-security
source_filename: recast-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.recastsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 21:41:16 2026 GMT\n  hsts: false\ndomains:\n- domain: recastsoftware.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"\\\"pki.goog; cansignhttpexchanges=yes\\\"\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/recast-software/security/recast-software-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automation
- Compliance
- IT Management
- Microsoft
---
