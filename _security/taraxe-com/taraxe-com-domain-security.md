---
api_specs:
- filename: taraxe-com-openapi-generated.yml
  format: yaml
  label: Taraxe API
  slug: taraxe-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taraxe-com/openapi/_ae-authored/taraxe-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: true
  domain: taraxe.com
  spf: true
hosts:
- cert_expires: Jan  7 17:24:20 2027 GMT
  host: taraxe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taraxe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taraxe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Taraxe
provider_slug: taraxe-com
slug: taraxe-com-domain-security
source_filename: taraxe-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taraxe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 17:24:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: taraxe.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/taraxe-com/security/taraxe-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Entrepreneurship
- Automation
- France
- SaaS
---
