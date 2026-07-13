---
api_specs:
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Campaigns API
  slug: sertifier-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Credentials API
  slug: sertifier-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Designs API
  slug: sertifier-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Credential Details API
  slug: sertifier-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Email Templates API
  slug: sertifier-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Recipients API
  slug: sertifier-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Attributes API
  slug: sertifier-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
- filename: sertifier-openapi.yml
  format: yaml
  label: Sertifier Webhooks API
  slug: sertifier-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/openapi/sertifier-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sertifier.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiary.io
  spf: true
hosts:
- cert_expires: Dec 25 13:06:51 2026 GMT
  host: sertifier.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: sertifier.docs.apiary.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 13:06:51 2026 GMT
  host: b2b.sertifier.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sertifier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sertifier, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sertifier
provider_slug: sertifier
slug: sertifier-domain-security
source_filename: sertifier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sertifier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 13:06:51 2026 GMT\n  hsts: false\n- host: sertifier.docs.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\n- host: b2b.sertifier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 13:06:51 2026 GMT\n  hsts: false\ndomains:\n- domain: sertifier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apiary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/security/sertifier-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Digital Credentials
- Certificates
- Badges
- Open Badges
- Verifiable Credentials
- Credentialing
- EdTech
---
