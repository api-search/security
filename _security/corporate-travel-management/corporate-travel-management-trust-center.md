---
certifications: []
description: ''
kind: trust-center
layout: security
name: Corporate Travel Management Trust Center
name_suffix: Trust Center
overview: Corporate Travel Management maintains a public trust center covering its security and compliance posture.
provider_name: Corporate Travel Management
provider_slug: corporate-travel-management
slug: corporate-travel-management-trust-center
source_filename: corporate-travel-management-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nprobe: true\nurl: https://trust.travelctm.com/\nplatform: UpGuard Trust Center\npublished: false\nstatus: provisioned-not-published\ncertifications: []\nevidence:\n- source: https://trust.travelctm.com/\n  status: 200\n  finding: >-\n    Serves the UpGuard Trust Center shell (title \"UpGuard Trust Center\", react-root, CR_HOSTNAME\n    cyber-risk.upguard.com). The page renders entirely client-side.\n- source: https://trust.travelctm.com/api/trustpage/public/v1/\n  status: 200\n  finding: 'Returns {\"status\":\"not_published\"} — the trust page content has never been published.'\n- source: https://au.travelctm.com/payment-card-industry-data-security-standard/\n  status: 200\n  finding: >-\n    The one compliance artefact CTM does publish is a PCI DSS v3.2.1 SAQ D Attestation of\n    Compliance PDF, dated April 2021. Captured in\n    conformance/corporate-travel-management-conformance.yml.\nnotes: >-\n  Recorded as a negative-but-notable\
  \ finding: Corporate Travel Management has stood up a branded\n  UpGuard trust-centre host on its own domain and left it unpublished, so there is no public\n  security posture, certification list, sub-processor list or document request flow. No TrustCenter\n  pointer is wired into apis.yml, because nothing is published behind the host. Re-probe the API\n  endpoint above on the next enrichment round — a status change from not_published is the signal\n  that CTM has opened its trust centre.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corporate-travel-management/refs/heads/main/security/corporate-travel-management-trust-center.yml
summary_line: trust center published
tags:
- Travel
- Australia
- Corporate Travel
- Travel Management Company
- Aviation
- NDC
- Distribution
- Booking
- Hotels
- Meetings and Events
trust_url: https://trust.travelctm.com/
---
