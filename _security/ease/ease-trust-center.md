---
api_specs:
- filename: ease-discovery-api-openapi.yml
  format: yaml
  label: Ease Discovery API
  slug: ease-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-discovery-api-openapi.yml
- filename: ease-events-api-openapi.yml
  format: yaml
  label: Ease Events API
  slug: ease-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-events-api-openapi.yml
- filename: ease-incidents-api-openapi.yml
  format: yaml
  label: Ease Incidents API
  slug: ease-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-incidents-api-openapi.yml
- filename: ease-maintenance-api-openapi.yml
  format: yaml
  label: Ease Maintenance API
  slug: ease-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-maintenance-api-openapi.yml
- filename: ease-marketplace-api-openapi.yml
  format: yaml
  label: Ease Marketplace API
  slug: ease-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-marketplace-api-openapi.yml
- filename: ease-media-api-openapi.yml
  format: yaml
  label: Ease Media API
  slug: ease-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-media-api-openapi.yml
- filename: ease-oembed-api-openapi.yml
  format: yaml
  label: Ease O Embed API
  slug: ease-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-oembed-api-openapi.yml
- filename: ease-pages-api-openapi.yml
  format: yaml
  label: Ease Pages API
  slug: ease-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-pages-api-openapi.yml
- filename: ease-posts-api-openapi.yml
  format: yaml
  label: Ease Posts API
  slug: ease-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-posts-api-openapi.yml
- filename: ease-search-api-openapi.yml
  format: yaml
  label: Ease Search API
  slug: ease-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-search-api-openapi.yml
- filename: ease-status-api-openapi.yml
  format: yaml
  label: Ease Status API
  slug: ease-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-status-api-openapi.yml
- filename: ease-taxonomy-api-openapi.yml
  format: yaml
  label: Ease Taxonomy API
  slug: ease-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-taxonomy-api-openapi.yml
- filename: ease-testimonials-api-openapi.yml
  format: yaml
  label: Ease Testimonials API
  slug: ease-testimonials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-testimonials-api-openapi.yml
certifications:
- SOC 2 Type II
- HITRUST
- HIPAA
- GDPR
- CCPA
- 23 NYCRR 500 (NYDFS)
- NIST
description: ''
kind: trust-center
layout: security
name: Ease Trust Center
name_suffix: Trust Center
overview: Ease maintains a public trust center documenting SOC 2 Type II, HITRUST, HIPAA, GDPR, CCPA, 23 NYCRR 500 (NYDFS), and NIST compliance.
provider_name: Ease
provider_slug: ease
slug: ease-trust-center
source_filename: ease-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nprobe: true\nsource: https://www.ease.com/product/security/\nurl: https://www.employeenavigator.com/security/\nfirst_party: false\nnote: >-\n  Ease hosts no trust center of its own. trust.ease.com and security.ease.com do not resolve to\n  a trust page, and the automated probe over ease.com/trust, /security and /compliance found no\n  qualifying page. What Ease does publish is a security page at\n  https://www.ease.com/product/security/ which states that, following Employee Navigator's\n  completion of the Ease acquisition on 2023-04-03, Ease \"now falls under Employee Navigator's\n  security program\" and links to the Employee Navigator security page. That page is therefore\n  the operative trust/compliance surface for Ease, recorded here with the ownership attribution\n  made explicit.\nease_security_page: https://www.ease.com/product/security/\ncertifications:\n- SOC 2 Type II\n- HITRUST\n- HIPAA\n- GDPR\n- CCPA\n- 23 NYCRR 500\
  \ (NYDFS)\n- NIST\nease_claimed_certifications:\n- HIPAA\n- SOC 2 Type II\n- HITRUST CSF Certification\nease_claimed_source: https://www.ease.com/product/security/sso/\naudit_cadence: annual\naudit_statement: >-\n  \"Employee Navigator is audited annually for SOC2 Type II, HITRUST, NIST, GDPR, 23 NYCRR 500,\n  and CCPA.\" - https://www.employeenavigator.com/security/\ncontrols_published:\n- Personnel security and third-party background checks\n- Least-privilege access management\n- Third-party vulnerability and penetration testing (stated on the Ease SSO page)\n- Mandatory two-factor authentication for all Ease users\n- Okta SAML single sign-on on the Ease Enterprise package\nevidence:\n- source: https://www.ease.com/product/security/\n  keywords: [security program, employee navigator, data privacy and security by design]\n- source: https://www.ease.com/product/security/sso/\n  keywords: [hipaa, soc 2 type ii, hitrust, hitrust csf certification, two-factor authentication, penetration testing]\n\
  - source: https://www.employeenavigator.com/security/\n  keywords: [soc 2 type ii, hitrust, nist, gdpr, 23 nycrr 500, ccpa, hipaa, compliance certifications and attestations]\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No security.txt, no bug bounty, no security@ contact and no responsible-disclosure page was\n    found for ease.com or employeenavigator.com. See security/ease-domain-security.yml for the\n    probed transport posture. Security inquiries are routed through the Ease support team.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/security/ease-trust-center.yml
summary_line: SOC 2 Type II, HITRUST, HIPAA, GDPR, CCPA, 23 NYCRR 500 (NYDFS), NIST
tags:
- Insurance
- United States
- Employee Benefits
- Benefits Administration
- Group Benefits
- Health Insurance
- Insurtech
- Brokers
- Enrollment
- EDI
- Payroll
- Human Resources
- Marketplace
- Status
trust_url: https://www.employeenavigator.com/security/
---
