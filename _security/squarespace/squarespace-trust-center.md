---
api_specs:
- filename: squarespace-orders-api-openapi.yml
  format: yaml
  label: Squarespace Orders API
  slug: squarespace-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-orders-api-openapi.yml
- filename: squarespace-products-api-openapi.yml
  format: yaml
  label: Squarespace Products API
  slug: squarespace-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-products-api-openapi.yml
- filename: squarespace-inventory-api-openapi.yml
  format: yaml
  label: Squarespace Inventory API
  slug: squarespace-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-inventory-api-openapi.yml
- filename: squarespace-profiles-api-openapi.yml
  format: yaml
  label: Squarespace Profiles API
  slug: squarespace-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-profiles-api-openapi.yml
- filename: squarespace-transactions-api-openapi.yml
  format: yaml
  label: Squarespace Transactions API
  slug: squarespace-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-transactions-api-openapi.yml
- filename: squarespace-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Squarespace Webhook Subscriptions API
  slug: squarespace-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-webhook-subscriptions-api-openapi.yml
- filename: squarespace-site-api-openapi.yml
  format: yaml
  label: Squarespace Site API
  slug: squarespace-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-site-api-openapi.yml
- filename: squarespace-commerce-api-v2-openapi.json
  format: json
  label: Squarespace Commerce API
  slug: squarespace-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/openapi/squarespace-commerce-api-v2-openapi.json
certifications:
- named
- note
description: ''
kind: trust-center
layout: security
name: Squarespace Trust Center
name_suffix: Trust Center
overview: Squarespace maintains a public trust center documenting named and note compliance.
provider_name: Squarespace
provider_slug: squarespace
slug: squarespace-trust-center
source_filename: squarespace-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.squarespace.com/security\nprovider: Squarespace\nproviderId: squarespace\ntrust_center:\n  exists: false\n  url: null\n  note: >-\n    Squarespace operates no trust center. There is no portal publishing audit reports, no\n    certification index, and no document request flow. probe-security-programs.py returned\n    trust=none on 2026-08-13 and a manual search confirmed it.\nsecurity_page:\n  url: https://www.squarespace.com/security\n  status: 200\n  audience: merchants\n  machine_readable: false\n  note: >-\n    A marketing page aimed at site owners, not a security posture disclosure aimed at auditors or\n    integrators. It covers automatic SSL on customer domains, platform monitoring, and payment\n    compliance, and links no evidence.\ncertifications:\n  named: []\n  note: >-\n    No SOC 2, ISO 27001, HIPAA or FedRAMP status is published anywhere on squarespace.com. No audit\n    report, attestation letter,\
  \ bridge letter or certificate is offered under NDA or otherwise.\ncompliance_claims:\n  - standard: PCI-DSS\n    claim: >-\n      \"All of Squarespace's built-in payment processor integrations are compliant with PCI-DSS.\n      Sensitive card data is never handled by Squarespace. It goes directly to the payment\n      processor's servers; Squarespace doesn't have access to this information.\"\n    scope: payment-processor-integrations\n    attests_own_environment: false\n    assessment: >-\n      This is a SCOPE-LIMITING statement, not a Squarespace attestation. It asserts that the\n      third-party processors are compliant and that Squarespace is out of card-data scope by design.\n      No SAQ type, no AOC, no assessor and no compliance level is named. Read as a descoping claim,\n      not a certification.\n    source: https://www.squarespace.com/security\n  - standard: 'global privacy and payment standards'\n    claim: >-\n      \"Squarespace keeps your site constantly monitored and\
  \ in compliance with global privacy and\n      payment standards.\"\n    scope: unspecified\n    attests_own_environment: false\n    assessment: Unnamed standards, no evidence, no scope. Not a usable compliance signal.\n    source: https://www.squarespace.com/security\ncompliance_pointer_emitted: false\ncompliance_pointer_rationale: >-\n  No `type: Compliance` pointer is wired into apis.yml for this provider. The only named standard on\n  the page is PCI-DSS, and Squarespace names it specifically to say the requirement lands on its\n  payment processors rather than on Squarespace. Crediting that as a published compliance program\n  would report a posture Squarespace has not claimed.\nvulnerability_disclosure:\n  published: true\n  detail: security/squarespace-vulnerability-disclosure.yml\n  url: https://www.squarespace.com/vulnerability-reporting\n  security_txt: well-known/squarespace-security.txt\n  bug_bounty:\n    platform: null\n    note: >-\n      No HackerOne, Bugcrowd or Intigriti\
  \ program was located. The security.txt Contact and Policy\n      both resolve to Squarespace's own vulnerability-reporting page rather than a bounty platform.\nsubdomain_caution:\n  finding: >-\n    https://trust.squarespace.com returns HTTP 200 and is NOT a Squarespace trust center — it is a\n    CUSTOMER SITE, a facilitation consultancy trading as \"Trust\" that built its website on\n    Squarespace.\n  why_it_matters: >-\n    Squarespace hosts customer sites on *.squarespace.com subdomains, so a 200 on a plausible\n    subdomain (trust., security., status-like names) proves nothing about Squarespace itself. Any\n    automated trust-center or well-known probe against this provider must read the page content\n    before recording a hit. Recorded here so a later pass does not re-discover this and file it as a\n    Squarespace trust center.\n  probed: '2026-08-13'\nevidence:\n  - url: https://www.squarespace.com/security\n    status: 200\n    note: Merchant-facing security marketing page;\
  \ names PCI-DSS only as a processor-scope claim.\n  - url: https://trust.squarespace.com\n    status: 200\n    note: Customer site, not Squarespace. Content is a consultancy's marketing site.\n  - url: https://www.squarespace.com/trust\n    status: 404\n  - url: https://www.squarespace.com/vulnerability-reporting\n    status: 200\n  - url: https://www.squarespace.com/.well-known/security.txt\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squarespace/refs/heads/main/security/squarespace-trust-center.yml
summary_line: named, note
tags:
- Commerce
- E-Commerce
- Marketing
- Payments
- Retail
- Website Builder
- Webhook
trust_url: ''
---
