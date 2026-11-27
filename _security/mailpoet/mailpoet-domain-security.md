---
api_specs:
- filename: mailpoet-openapi-generated.yml
  format: yaml
  label: Mailpoet API
  slug: mailpoet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailpoet/openapi/_ae-authored/mailpoet-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mailpoet.com
  spf: true
hosts:
- cert_expires: Jan 12 12:58:00 2027 GMT
  host: mailpoet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailpoet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailpoet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mailpoet
provider_slug: mailpoet
slug: mailpoet-domain-security
source_filename: mailpoet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailpoet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 12:58:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailpoet.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mailpoet/security/mailpoet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- WordPress
- Newsletters
- Open Source
- Software-as-a-Service
---
