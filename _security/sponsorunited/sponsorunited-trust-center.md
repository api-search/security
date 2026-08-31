---
api_specs:
- filename: sponsorunited-api-openapi.json
  format: json
  label: SponsorUnited API
  slug: sponsorunited-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sponsorunited/refs/heads/main/openapi/sponsorunited-api-openapi.json
certifications:
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Sponsorunited Trust Center
name_suffix: Trust Center
overview: SponsorUnited maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: SponsorUnited
provider_slug: sponsorunited
slug: sponsorunited-trust-center
source_filename: sponsorunited-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://www.sponsorunited.com/security\ntrust_center:\n  url: https://trust.sponsorunited.com/\n  platform: Vanta\n  http_status: 200\n  machine_readable: false\n  note: The trust center is a Vanta-hosted single-page app; its certification list is\n    rendered client-side and no anonymous API returns it (api.vanta.com returns 401).\n    Certifications below were therefore read from the provider's own security page,\n    which states them in prose.\nsecurity_page:\n  url: https://www.sponsorunited.com/security\n  http_status: 200\ncertifications:\n- name: SOC 2 Type II\n  status: attested\n  evidence: '\"SponsorUnited maintains a SOC 2 Type II attestation\" — https://www.sponsorunited.com/security'\n  report_availability: Report available via the trust center / on request.\n- name: GDPR\n  status: compliance certification claimed\n  evidence: '\"and a GDPR compliance certification\" — https://www.sponsorunited.com/security'\n\
  program:\n  penetration_testing:\n    cadence: annual\n    partner: Rhymetec\n    scope: All product and cloud infrastructure in scope; source code provided to testers.\n    reports: Summary penetration test reports available upon request.\n  vulnerability_scanning:\n  - Static analysis (SAST) on pull requests and ongoing\n  - Malicious dependency scanning\n  - Periodic network vulnerability scanning\n  - Software composition analysis (SCA)\n  - Dynamic analysis (DAST) of running applications\n  - External attack surface management (EASM)\n  data_protection:\n    at_rest: All datastores with customer data and S3 buckets encrypted at rest; sensitive\n      collections and tables additionally use row-level encryption.\n    note: The published page repeats the at-rest paragraph verbatim under \"Data in transit\"\n      and \"Secret management\", so no distinct in-transit or secret-management control is\n      actually stated. Recorded as published, not as three separate controls.\nvulnerability_disclosure:\n\
  \  published: false\n  note: No SponsorUnited-operated /.well-known/security.txt, no security@ address, no bug\n    bounty and no responsible-disclosure page were found. The only security.txt reachable\n    on a SponsorUnited hostname is Intercom's, served on the vendor-hosted help center\n    (help.sponsorunited.com) and canonical to app.intercom.com — it is Intercom's document,\n    not SponsorUnited's, and is not credited here.\n  general_contact: info@sponsorunited.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sponsorunited/refs/heads/main/security/sponsorunited-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Company
- Sponsorship
- Sports
- Entertainment
- Marketing
- Advertising
- Media
- Data
- Analytics
- Market Intelligence
- Software-as-a-Service
- Partnerships
trust_url: ''
---
