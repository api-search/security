---
api_specs:
- filename: google-contacts-contactgroups-api-openapi.yml
  format: yaml
  label: Google People API ContactGroups API
  slug: google-contacts-contactgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-contacts/refs/heads/main/openapi/google-contacts-contactgroups-api-openapi.yml
- filename: google-contacts-people-api-openapi.yml
  format: yaml
  label: Google People API People API
  slug: google-contacts-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-contacts/refs/heads/main/openapi/google-contacts-people-api-openapi.yml
- filename: google-contacts-people-createcontact-api-openapi.yml
  format: yaml
  label: Google People API People:createContact API
  slug: google-contacts-people-createcontact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-contacts/refs/heads/main/openapi/google-contacts-people-createcontact-api-openapi.yml
- filename: google-contacts-people-searchcontacts-api-openapi.yml
  format: yaml
  label: Google People API People:searchContacts API
  slug: google-contacts-people-searchcontacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-contacts/refs/heads/main/openapi/google-contacts-people-searchcontacts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: people.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Contacts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google People API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google People API
provider_slug: google-contacts
slug: google-contacts-domain-security
source_filename: google-contacts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: people.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-contacts/refs/heads/main/security/google-contacts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Address Book
- Contacts
- Directory
- Google
- People
- Profiles
---
