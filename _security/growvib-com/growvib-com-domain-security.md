---
api_specs:
- filename: growvib-com-agent-payments-api-openapi.yml
  format: yaml
  label: GrowVib Agent payments API
  slug: growvib-com-agent-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growvib-com/openapi/growvib-com-agent-payments-api-openapi.yml
- filename: growvib-com-catalog-api-openapi.yml
  format: yaml
  label: GrowVib Catalog API
  slug: growvib-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/growvib-com/openapi/growvib-com-catalog-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@growvib.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: growvib.com
  spf: true
hosts:
- cert_expires: Dec 25 07:16:24 2026 GMT
  host: growvib.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GrowVib Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GrowVib, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: GrowVib
provider_slug: growvib-com
slug: growvib-com-domain-security
source_filename: growvib-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: growvib.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 07:16:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: growvib.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@growvib.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/growvib-com/security/growvib-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SMM
- Social Media
- Marketing
- Automation
- Telegram
---
