---
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Grid Trust Center
name_suffix: Trust Center
overview: Grid maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Grid
provider_slug: grid
slug: grid-trust-center
source_filename: grid-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.withgrid.com/security\ntrust_center:\n  published: false\n  published_note: >-\n    There is no trust centre. trust.withgrid.com and security.withgrid.com do not resolve;\n    /trust returns 404. What Grid publishes is a single marketing-page-shaped /security page\n    plus one blog post announcing a completed audit. Recorded here because the certification\n    claim is real and named, not because a trust programme is published.\n  urls:\n    - url: https://www.withgrid.com/security\n      status: 200\n      title: Security\n    - url: https://www.withgrid.com/post/grid-is-now-soc-2-type-ii-compliant\n      status: 200\n      title: Grid is now SOC 2 Type II compliant\n    - url: https://www.withgrid.com/trust\n      status: 404\n      title: 'no trust centre'\ncertifications:\n  - name: SOC 2 Type II\n    status: completed\n    scope: >-\n      Grid's announcement describes the SOC 2 framework as covering security,\
  \ availability,\n      processing integrity, confidentiality and privacy, but does not state which trust\n      services criteria were in scope for its own audit.\n    auditor: null\n    auditor_note: Not named.\n    report_date: null\n    report_date_note: >-\n      Not stated in the announcement. The post is undated on the page as rendered.\n    report_access: >-\n      No self-serve request flow. The post directs readers to book a consultation at\n      https://www.withgrid.com/request-demo — a sales form, not a document request.\n    evidence: >-\n      \"Grid is pleased to announce that we have successfully completed our SOC 2 Type II\n      audit! This achievement underscores our dedication to maintaining the highest\n      standards of data security, availability, and confidentiality for our customers.\"\n    source: https://www.withgrid.com/post/grid-is-now-soc-2-type-ii-compliant\nsecurity_program:\n  hosting: Amazon Web Services\n  encryption_at_rest: true\n  encryption_in_transit:\
  \ true\n  key_management: AWS Key Management Service (KMS)\n  network_isolation: >-\n    \"we only allow access to our data through VPCs\"\n  aws_security_services:\n    - KMS\n    - GuardDuty\n    - Inspector\n  deployment: Containerised on AWS managed services\n  static_analysis: >-\n    \"high-quality static analysis tooling provided by Github\" run during development\n  vendor_management: >-\n    Grid states that \"all vendors that have access to any data are SOC 2 certified\". Note\n    this is a claim about VENDORS, and is separate from Grid's own SOC 2 Type II audit,\n    which is announced on the blog rather than on the security page.\n  third_party_penetration_testing: null\n  third_party_penetration_testing_note: Not mentioned.\n  subprocessor_list_published: false\n  incident_response_published: false\n  sso_available: true\n  sso_note: >-\n    SAML 2.0 SSO with Okta and Microsoft Entra ID —\n    https://help.saasgrid.com/articles/9859006764-setting-up-sso-for-saasgrid\nevidence_documents_public:\
  \ false\nvulnerability_disclosure:\n  published: false\n  security_contact: null\n  security_txt: false\n  bug_bounty: null\n  note: >-\n    NO DISCLOSURE CHANNEL EXISTS. /.well-known/security.txt returns 404 on every Grid host\n    (withgrid.com, www.withgrid.com, app.withgrid.com, api.saasgrid.com, app.saasgrid.com,\n    help.saasgrid.com). The /security page publishes no security@ address and no reporting\n    instructions. No programme was found on HackerOne, Bugcrowd or Intigriti by\n    probe-security-programs.py, which returned vdp=none. A researcher who finds a bug in\n    Grid has no published route to report it. NO Security or VulnerabilityDisclosure\n    pointer is emitted in apis.yml, because none is earned.\nnote: >-\n  The security posture and the certification are published in two different places and only\n  one of them is linked from the site navigation. The /security page — the page a buyer's\n  security team will actually open — never mentions Grid's own SOC 2 Type II.\
  \ That claim\n  lives only in a blog post reachable through the sitemap. A reader who checks /security\n  will conclude that only Grid's vendors are SOC 2 certified.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grid/refs/heads/main/security/grid-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Infrastructure
- Revenue Operations
- SaaS Metrics
- Billing
- Forecasting
- Financial Reporting
- FinOps
trust_url: ''
---
