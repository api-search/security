---
api_specs:
- filename: email-spam-tester-com-free-dns-tools-api-openapi.yml
  format: yaml
  label: Free Email Spam Tester Free DNS tools API
  slug: email-spam-tester-com-free-dns-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/email-spam-tester-com/openapi/email-spam-tester-com-free-dns-tools-api-openapi.yml
- filename: email-spam-tester-com-health-api-openapi.yml
  format: yaml
  label: Free Email Spam Tester Health API
  slug: email-spam-tester-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/email-spam-tester-com/openapi/email-spam-tester-com-health-api-openapi.yml
- filename: email-spam-tester-com-inbox-api-openapi.yml
  format: yaml
  label: Free Email Spam Tester Inbox API
  slug: email-spam-tester-com-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/email-spam-tester-com/openapi/email-spam-tester-com-inbox-api-openapi.yml
- filename: email-spam-tester-com-inbox-placement-api-openapi.yml
  format: yaml
  label: Free Email Spam Tester Inbox placement API
  slug: email-spam-tester-com-inbox-placement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/email-spam-tester-com/openapi/email-spam-tester-com-inbox-placement-api-openapi.yml
- filename: email-spam-tester-com-infra-checks-api-openapi.yml
  format: yaml
  label: Free Email Spam Tester Infra checks API
  slug: email-spam-tester-com-infra-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/email-spam-tester-com/openapi/email-spam-tester-com-infra-checks-api-openapi.yml
- filename: email-spam-tester-com-keys-api-openapi.yml
  format: yaml
  label: Free Email Spam Tester Keys API
  slug: email-spam-tester-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/email-spam-tester-com/openapi/email-spam-tester-com-keys-api-openapi.yml
- filename: email-spam-tester-com-tests-api-openapi.yml
  format: yaml
  label: Free Email Spam Tester Tests API
  slug: email-spam-tester-com-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/email-spam-tester-com/openapi/email-spam-tester-com-tests-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:tanichev@email-spam-tester.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: email-spam-tester.com
  spf: true
hosts:
- cert_expires: Dec 23 11:17:12 2026 GMT
  host: email-spam-tester.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Free Email Spam Tester Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Free Email Spam Tester, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Free Email Spam Tester
provider_slug: email-spam-tester-com
slug: email-spam-tester-com-domain-security
source_filename: email-spam-tester-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: email-spam-tester.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 11:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: email-spam-tester.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:tanichev@email-spam-tester.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/email-spam-tester-com/security/email-spam-tester-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email
- Deliverability
- Spam
- Testing
- Free
---
