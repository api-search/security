---
api_specs:
- filename: cvent-hospitality-cloud-housing-openapi.yml
  format: yaml
  label: Cvent Passkey RegLink API
  slug: passkey-reglink
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-housing-openapi.yml
- filename: cvent-hospitality-cloud-authentication-openapi.yml
  format: yaml
  label: Cvent Platform REST API (Hospitality)
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-authentication-openapi.yml
- filename: cvent-hospitality-cloud-rfp-management-openapi.yml
  format: yaml
  label: Cvent RFP Management API
  slug: rfp-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-management-openapi.yml
- filename: cvent-hospitality-cloud-rfp-requirements-openapi.yml
  format: yaml
  label: Cvent RFP Requirements API
  slug: rfp-requirements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml
- filename: cvent-hospitality-cloud-rfp-suppliers-openapi.yml
  format: yaml
  label: Cvent RFP Suppliers API
  slug: rfp-suppliers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml
- filename: cvent-hospitality-cloud-rfp-additional-details-openapi.yml
  format: yaml
  label: Cvent RFP Additional Details API
  slug: rfp-additional-details
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml
- filename: cvent-hospitality-cloud-proposal-drafts-openapi.yml
  format: yaml
  label: Cvent Proposal Draft API
  slug: proposal-drafts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml
- filename: cvent-hospitality-cloud-venue-profiles-openapi.yml
  format: yaml
  label: Cvent Venue Profiles API
  slug: venue-profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml
- filename: cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml
  format: yaml
  label: Cvent Venue Meeting Rooms API
  slug: venue-meeting-rooms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml
- filename: cvent-hospitality-cloud-meeting-requests-openapi.yml
  format: yaml
  label: Cvent Meeting Request API
  slug: meeting-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml
- filename: cvent-hospitality-cloud-travel-rfps-openapi.yml
  format: yaml
  label: Cvent Travel RFPs API
  slug: travel-rfps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml
- filename: cvent-hospitality-cloud-travel-suppliers-openapi.yml
  format: yaml
  label: Cvent Travel Suppliers API
  slug: travel-suppliers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml
- filename: cvent-hospitality-cloud-travel-accounts-openapi.yml
  format: yaml
  label: Cvent Travel Accounts API
  slug: travel-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml
- filename: cvent-hospitality-cloud-event-travel-openapi.yml
  format: yaml
  label: Cvent Event Travel API
  slug: event-travel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-event-travel-openapi.yml
- filename: cvent-hospitality-cloud-signatures-openapi.yml
  format: yaml
  label: Cvent Signatures API
  slug: signatures
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-signatures-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "comodo.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cvent.com
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: www.cvent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: developers.cvent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: api-platform.cvent.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cvent Hospitality Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cvent Hospitality Cloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cvent Hospitality Cloud
provider_slug: cvent-hospitality-cloud
slug: cvent-hospitality-cloud-domain-security
source_filename: cvent-hospitality-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-platform.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cvent.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/security/cvent-hospitality-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Catering
- Group Bookings
- Hospitality
- Hospitality Cloud
- Hotels
- Housing
- Authentication
- Passkey
- Reservations
- RFP
- Room Blocks
- Sales
- Sourcing
- Supplier Network
- Venues
---
