---
api_specs:
- filename: azion-api-openapi.json
  format: json
  label: azion-api API
  slug: azion-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azion/openapi/_original/azion-api-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "globalsign.com"
  - 0 iodef "mailto:noc@azion.com"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azion.com
  spf: true
hosts:
- cert_expires: Jan 17 21:51:10 2027 GMT
  host: azion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Azion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azion
provider_slug: azion
slug: azion-domain-security
source_filename: azion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 21:51:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azion.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 iodef \"mailto:noc@azion.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/azion/security/azion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Edge Computing
- Serverless
- Artificial Intelligence
- Cloud Infrastructure
- Platform
---
