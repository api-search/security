---
api_specs:
- filename: contactout-api-usage-stats-api-openapi.yml
  format: yaml
  label: ContactOut API Usage Stats API
  slug: contactout-api-usage-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-api-usage-stats-api-openapi.yml
- filename: contactout-campaigns-api-api-openapi.yml
  format: yaml
  label: ContactOut Campaigns API
  slug: contactout-campaigns-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-campaigns-api-api-openapi.yml
- filename: contactout-company-information-from-domains-api-openapi.yml
  format: yaml
  label: ContactOut Company information from domains API
  slug: contactout-company-information-from-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-company-information-from-domains-api-openapi.yml
- filename: contactout-company-search-api-api-openapi.yml
  format: yaml
  label: ContactOut Company Search API
  slug: contactout-company-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-company-search-api-api-openapi.yml
- filename: contactout-contact-checker-api-api-openapi.yml
  format: yaml
  label: ContactOut Contact Checker API
  slug: contactout-contact-checker-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-contact-checker-api-api-openapi.yml
- filename: contactout-contact-info-api-bulk-api-openapi.yml
  format: yaml
  label: ContactOut Contact Info API - Bulk API
  slug: contactout-contact-info-api-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-contact-info-api-bulk-api-openapi.yml
- filename: contactout-contact-info-api-single-api-openapi.yml
  format: yaml
  label: ContactOut Contact Info API - Single API
  slug: contactout-contact-info-api-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-contact-info-api-single-api-openapi.yml
- filename: contactout-decision-makers-api-api-openapi.yml
  format: yaml
  label: ContactOut Decision Makers API
  slug: contactout-decision-makers-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-decision-makers-api-api-openapi.yml
- filename: contactout-email-to-linkedin-api-api-openapi.yml
  format: yaml
  label: ContactOut Email to LinkedIn API
  slug: contactout-email-to-linkedin-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-email-to-linkedin-api-api-openapi.yml
- filename: contactout-email-verifier-api-api-openapi.yml
  format: yaml
  label: ContactOut Email Verifier API
  slug: contactout-email-verifier-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-email-verifier-api-api-openapi.yml
- filename: contactout-hashed-email-api-api-openapi.yml
  format: yaml
  label: ContactOut Hashed Email API
  slug: contactout-hashed-email-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-hashed-email-api-api-openapi.yml
- filename: contactout-linkedin-profile-api-api-openapi.yml
  format: yaml
  label: ContactOut LinkedIn Profile API
  slug: contactout-linkedin-profile-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-linkedin-profile-api-api-openapi.yml
- filename: contactout-people-count-api-api-openapi.yml
  format: yaml
  label: ContactOut People Count API
  slug: contactout-people-count-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-people-count-api-api-openapi.yml
- filename: contactout-people-enrich-api-api-openapi.yml
  format: yaml
  label: ContactOut People Enrich API
  slug: contactout-people-enrich-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-people-enrich-api-api-openapi.yml
- filename: contactout-people-search-api-api-openapi.yml
  format: yaml
  label: ContactOut People Search API
  slug: contactout-people-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-people-search-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: contactout.com
  spf: true
hosts:
- cert_expires: Dec  4 01:00:39 2026 GMT
  host: contactout.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contactout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ContactOut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ContactOut
provider_slug: contactout
slug: contactout-domain-security
source_filename: contactout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contactout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 01:00:39 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: contactout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/security/contactout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Contact Data
- Email Finder
- Data Enrichment
- People Search
- Company Search
- Email Verification
- Sales Intelligence
- Recruiting
- B2B Data
---
