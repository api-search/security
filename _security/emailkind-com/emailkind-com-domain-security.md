---
api_specs:
- filename: emailkind-com-classify-api-openapi.yml
  format: yaml
  label: EmailKind Classify API
  slug: emailkind-com-classify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailkind-com/openapi/emailkind-com-classify-api-openapi.yml
- filename: emailkind-com-signup-api-openapi.yml
  format: yaml
  label: EmailKind Signup API
  slug: emailkind-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailkind-com/openapi/emailkind-com-signup-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.cloudflare.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:hello@emailkind.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: emailkind.com
  spf: true
hosts:
- cert_expires: Jan  9 23:23:12 2027 GMT
  host: emailkind.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EmailKind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmailKind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: EmailKind
provider_slug: emailkind-com
slug: emailkind-com-domain-security
source_filename: emailkind-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailkind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:23:12 2027 GMT\n  hsts: false\ndomains:\n- domain: emailkind.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.cloudflare.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:hello@emailkind.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/emailkind-com/security/emailkind-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Email
- Email Verification
- Data Enrichment
- Software-as-a-Service
---
