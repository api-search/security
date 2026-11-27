---
api_specs:
- filename: docracy-io-openapi-generated.yml
  format: yaml
  label: Docracy API
  slug: docracy-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docracy-io/openapi/_ae-authored/docracy-io-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: docracy.io
  spf: true
hosts:
- cert_expires: Dec 16 20:19:55 2026 GMT
  host: docracy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docracy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docracy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Docracy
provider_slug: docracy-io
slug: docracy-io-domain-security
source_filename: docracy-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docracy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 20:19:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: docracy.io\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/docracy-io/security/docracy-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- E-Signature
- Free
- Document Automation
---
