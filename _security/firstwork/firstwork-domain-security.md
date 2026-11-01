---
api_specs:
- filename: firstwork-openapi-generated.yml
  format: yaml
  label: Firstwork API
  slug: firstwork-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firstwork/openapi/_ae-authored/firstwork-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: firstwork.com
  spf: true
hosts:
- cert_expires: Dec 27 02:03:18 2026 GMT
  host: www.firstwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firstwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firstwork, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Firstwork
provider_slug: firstwork
slug: firstwork-domain-security
source_filename: firstwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firstwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 02:03:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: firstwork.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/firstwork/security/firstwork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- HR
- Frontline
- Automation
- Compliance
---
