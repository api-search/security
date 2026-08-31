---
api_specs:
- filename: brandfolder-assets-api-openapi.yml
  format: yaml
  label: Brandfolder Assets API
  slug: brandfolder-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-assets-api-openapi.yml
- filename: brandfolder-attachments-api-openapi.yml
  format: yaml
  label: Brandfolder Attachments API
  slug: brandfolder-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-attachments-api-openapi.yml
- filename: brandfolder-binary-upload-api-openapi.yml
  format: yaml
  label: Brandfolder Binary Upload API
  slug: brandfolder-binary-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-binary-upload-api-openapi.yml
- filename: brandfolder-brandfolders-api-openapi.yml
  format: yaml
  label: Brandfolder Brandfolders API
  slug: brandfolder-brandfolders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-brandfolders-api-openapi.yml
- filename: brandfolder-collections-api-openapi.yml
  format: yaml
  label: Brandfolder Collections API
  slug: brandfolder-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-collections-api-openapi.yml
- filename: brandfolder-custom-fields-api-openapi.yml
  format: yaml
  label: Brandfolder Custom Fields API
  slug: brandfolder-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-custom-fields-api-openapi.yml
- filename: brandfolder-invitations-api-openapi.yml
  format: yaml
  label: Brandfolder Invitations API
  slug: brandfolder-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-invitations-api-openapi.yml
- filename: brandfolder-labels-api-openapi.yml
  format: yaml
  label: Brandfolder Labels API
  slug: brandfolder-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-labels-api-openapi.yml
- filename: brandfolder-organizations-api-openapi.yml
  format: yaml
  label: Brandfolder Organizations API
  slug: brandfolder-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-organizations-api-openapi.yml
- filename: brandfolder-sections-api-openapi.yml
  format: yaml
  label: Brandfolder Sections API
  slug: brandfolder-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-sections-api-openapi.yml
- filename: brandfolder-tags-api-openapi.yml
  format: yaml
  label: Brandfolder Tags API
  slug: brandfolder-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-tags-api-openapi.yml
- filename: brandfolder-user-permissions-api-openapi.yml
  format: yaml
  label: Brandfolder User Permissions API
  slug: brandfolder-user-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-user-permissions-api-openapi.yml
- filename: brandfolder-webhooks-api-openapi.yml
  format: yaml
  label: Brandfolder Webhooks API
  slug: brandfolder-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@smartsheet.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brandfolder.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@smartsheet.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartsheet.com
  spf: true
hosts:
- cert_expires: Sep 26 03:51:50 2026 GMT
  host: brandfolder.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:08:13 2026 GMT
  host: developers.smartsheet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brandfolder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandfolder, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brandfolder
provider_slug: brandfolder
slug: brandfolder-domain-security
source_filename: brandfolder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brandfolder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:51:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.smartsheet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:08:13 2026 GMT\n  hsts: false\ndomains:\n- domain: brandfolder.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@smartsheet.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: smartsheet.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@smartsheet.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/security/brandfolder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Asset Management
- DAM
- Brand Management
- Assets
- Media
- Collection
- Smartsheet
---
