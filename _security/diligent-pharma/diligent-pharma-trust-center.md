---
certifications: []
description: 'Diligent Pharma publishes a trust center on its own subdomain, https://trust.diligentpharma.com/ (HTTP 200), running the HyperComply Trust Center product. The surface is real and provider-controlled, but its contents are rendered entirely client-side: the served HTML is a shell titled "HyperComply" and every section is fetched afterwards through an Apollo GraphQL client, so an unauthenticated fetch returns no certification names, no framework list, no subprocessor list and no downloadable documents. Presence is recorded here; NO certification is claimed, because none could be read.'
kind: trust-center
layout: security
name: Diligent Pharma Trust Center
name_suffix: Trust Center
overview: Diligent Pharma maintains a public trust center covering its security and compliance posture.
provider_name: Diligent Pharma
provider_slug: diligent-pharma
slug: diligent-pharma-trust-center
source_filename: diligent-pharma-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://trust.diligentpharma.com/\ndescription: >-\n  Diligent Pharma publishes a trust center on its own subdomain,\n  https://trust.diligentpharma.com/ (HTTP 200), running the HyperComply Trust Center\n  product. The surface is real and provider-controlled, but its contents are rendered\n  entirely client-side: the served HTML is a shell titled \"HyperComply\" and every\n  section is fetched afterwards through an Apollo GraphQL client, so an unauthenticated\n  fetch returns no certification names, no framework list, no subprocessor list and no\n  downloadable documents. Presence is recorded here; NO certification is claimed,\n  because none could be read.\ntrust_center:\n  url: https://trust.diligentpharma.com/\n  http_status: 200\n  platform: HyperComply\n  platform_evidence: >-\n    Page title \"HyperComply\"; assets preloaded from assets.hypercomply.com; the\n    Diligent360 application bundle also references https://diligent.hypercomply.com.\n\
  \  content_machine_readable: false\n  content_readable_reason: >-\n    JavaScript-rendered SPA backed by GraphQL (/api/1/graphql); server HTML contains\n    no trust content.\ncertifications: []\ncertifications_verified: false\nframeworks_referenced_elsewhere:\n  note: >-\n    Read from https://www.diligentpharma.com/privacy-policy and\n    https://www.diligentpharma.com/expertise/regulatory-standards, not from the trust\n    center itself.\n  frameworks:\n    - GDPR\n    - CCPA / CPRA\n    - 21 CFR Part 11\n    - EU Annex 11\n    - ICH E6 (R3)\ncontacts:\n  - purpose: privacy\n    email: privacy@diligentpharma.com\n    source: https://www.diligentpharma.com/privacy-policy\nvulnerability_disclosure:\n  published: false\n  evidence:\n    - url: https://www.diligentpharma.com/.well-known/security.txt\n      status: 404\n    - url: https://www.diligentpharma.com/security\n      status: 404\n  note: >-\n    No security.txt, no responsible-disclosure page, and no bug bounty program\n    (HackerOne\
  \ / Bugcrowd / Intigriti) was found. No VulnerabilityDisclosure or\n    Security pointer was emitted.\ngaps:\n  - Serve the trust center content server-rendered, or publish a machine-readable\n    summary, so the certifications the company holds are discoverable without executing\n    JavaScript.\n  - Publish an RFC 9116 /.well-known/security.txt naming a security contact and policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diligent-pharma/refs/heads/main/security/diligent-pharma-trust-center.yml
summary_line: trust center published
tags:
- Company
- Clinical Trials
- Life Sciences
- Pharmaceuticals
- Biotechnology
- Vendor Management
- Risk Management
- Quality Management
- Compliance
- GxP
- Auditing
- SaaS
trust_url: ''
---
