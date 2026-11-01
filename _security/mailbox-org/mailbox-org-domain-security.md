---
api_specs:
- filename: mailbox-org-openapi-generated.yml
  format: yaml
  label: mailbox.org API
  slug: mailbox-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbox-org/openapi/_ae-authored/mailbox-org-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@heinlein-support.de"
  - 0 iodef "mailto:mail@heinlein-support.de"
  - 0 issue "swisssign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mailbox.org
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: mailbox.org
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailbox Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mailbox.org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: mailbox.org
provider_slug: mailbox-org
slug: mailbox-org-domain-security
source_filename: mailbox-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailbox.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: mailbox.org\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@heinlein-support.de\"\n  - 0 iodef \"mailto:mail@heinlein-support.de\"\n  - 0 issue \"swisssign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mailbox-org/security/mailbox-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email
- Collaboration
- Privacy
- GDPR
- German
---
