---
api_specs:
- filename: awin-affiliate-accounts-api-openapi.yml
  format: yaml
  label: Awin Accounts API
  slug: awin-affiliate-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-accounts-api-openapi.yml
- filename: awin-affiliate-commission-groups-api-openapi.yml
  format: yaml
  label: Awin Commission Groups API
  slug: awin-affiliate-commission-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-commission-groups-api-openapi.yml
- filename: awin-affiliate-programmes-api-openapi.yml
  format: yaml
  label: Awin Programmes API
  slug: awin-affiliate-programmes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-programmes-api-openapi.yml
- filename: awin-affiliate-reports-api-openapi.yml
  format: yaml
  label: Awin Reports API
  slug: awin-affiliate-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-reports-api-openapi.yml
- filename: awin-affiliate-transactions-api-openapi.yml
  format: yaml
  label: Awin Transactions API
  slug: awin-affiliate-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-transactions-api-openapi.yml
certifications:
- ISO 27001
- GDPR
description: Awin has no dedicated trust centre subdomain - trust.awin.com does not resolve and www.awin.com/gb/security returns 404. What it publishes instead is an "Awin's Approach to Information Security" legal page carrying a named ISO 27001 certification claim and a GDPR processing statement, plus a separate Compliance page and a Privacy page. There is no evidence portal, no downloadable audit report and no subprocessor list found.
kind: trust-center
layout: security
name: Awin Affiliate Trust Center
name_suffix: Trust Center
overview: Awin maintains a public trust center documenting ISO 27001 and GDPR compliance.
provider_name: Awin
provider_slug: awin-affiliate
slug: awin-affiliate-trust-center
source_filename: awin-affiliate-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://www.awin.com/gb/legal/information-security\ndescription: >-\n  Awin has no dedicated trust centre subdomain - trust.awin.com does not resolve\n  and www.awin.com/gb/security returns 404. What it publishes instead is an\n  \"Awin's Approach to Information Security\" legal page carrying a named ISO 27001\n  certification claim and a GDPR processing statement, plus a separate Compliance\n  page and a Privacy page. There is no evidence portal, no downloadable audit\n  report and no subprocessor list found.\ncertifications:\n- ISO 27001\n- GDPR\ncertification_detail:\n- name: ISO/IEC 27001\n  claimed: true\n  statement: >-\n    \"We're proud to hold the ISO 27001 certification. This means our information\n    security management system has been thoroughly audited and meets strict\n    requirements for protecting the confidentiality, integrity and availability\n    of your information. We have successfully completed\
  \ external, independent\n    audits to attest to our compliance with the ISO 27001 standard.\"\n  certificate_available: false\n  note: Certificate number, issuing body and scope are not published on the page.\n- name: GDPR\n  claimed: true\n  statement: >-\n    \"We meet our legal obligations under the EU General Data Protection\n    Regulation (GDPR) by using adequate technical and organisational measures.\"\n  certificate_available: false\npages:\n- url: https://www.awin.com/gb/legal/information-security\n  role: information security / certifications\n  status: 200\n- url: https://www.awin.com/gb/compliance\n  role: compliance management and sustainability\n  status: 200\n- url: https://www.awin.com/gb/privacy\n  role: privacy policy\n  status: 200\n- url: https://www.awin.com/gb/site-notice\n  role: site notice / legal imprint\n  status: 200\nwhistleblowing:\n  url: http://www.bkms-system.net/awin\n  note: >-\n    Awin links an external BKMS whistleblowing system from the site footer\
  \ -\n    a governance channel distinct from the security vulnerability channel.\nevidence:\n- source: https://www.awin.com/gb/legal/information-security\n  keywords:\n  - iso 27001\n  - gdpr\n  - information security\n  - independent audits\nabsent:\n- trust.awin.com (does not resolve)\n- https://www.awin.com/gb/security (404)\n- SOC 2 report\n- Public subprocessor list\n- Security evidence / document request portal\nx-evidence:\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/security/awin-affiliate-trust-center.yml
summary_line: ISO 27001, GDPR
tags:
- Affiliate Marketing
- Advertising
- Publishers
- Advertisers
- Transactions
- Reporting
- Commissions
- Performance Marketing
trust_url: https://www.awin.com/gb/legal/information-security
---
