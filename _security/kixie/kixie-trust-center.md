---
certifications: []
description: Kixie publishes a public trust page at https://www.kixie.com/security/, titled "Kixie Security, Privacy, and Trust Resources" and self-described as "a routing page for public trust information". It routes to the privacy policy, terms of use, status page and security contact. It publishes ZERO certifications, and says so on purpose.
kind: trust-center
layout: security
name: Kixie Trust Center
name_suffix: Trust Center
overview: Kixie maintains a public trust center covering its security and compliance posture.
provider_name: Kixie
provider_slug: kixie
slug: kixie-trust-center
source_filename: kixie-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://www.kixie.com/security/\ndocs: https://www.kixie.com/security/\n\nname: Kixie trust center\ndescription: >-\n  Kixie publishes a public trust page at https://www.kixie.com/security/, titled \"Kixie Security,\n  Privacy, and Trust Resources\" and self-described as \"a routing page for public trust\n  information\". It routes to the privacy policy, terms of use, status page and security contact.\n  It publishes ZERO certifications, and says so on purpose.\n\npublished: true\nurl: https://www.kixie.com/security/\nprobed:\n  url: https://www.kixie.com/security/\n  http_status: 200\n  fetched: '2026-08-12'\nplatform: first-party HTML page\nthird_party_trust_platform: none\nlast_reviewed: '2026-08-03'\n\ncertifications: []\ncertification_count: 0\ncertifications_finding: >-\n  No SOC 2 Type I or II, ISO 27001, ISO 27701, PCI DSS, HIPAA/BAA, FedRAMP, StateRAMP, CSA STAR\n  or Cyber Essentials claim appears anywhere on Kixie's\
  \ public surface. The page states the\n  omission is deliberate: \"This public page intentionally does not claim a certification, audit\n  result, hosting architecture, retention period, or control that has not been confirmed for\n  publication.\"\n\nsubresources_published:\n- name: Privacy Policy\n  url: https://www.kixie.com/privacy/\n  note: Kixie names this as the authoritative description of its safeguards and data handling.\n- name: Terms of Use\n  url: https://www.kixie.com/terms/\n  note: Named as the location of contractual terms.\n- name: Status page\n  url: https://status.kixie.com/\n  note: Availability and incident history; machine-readable via the Statuspage v2 API.\n- name: Security contact\n  value: security@kixie.com\n\nnot_published:\n- SOC 2 or ISO report (even under NDA via a self-serve request flow)\n- subprocessor list\n- data-residency or hosting-architecture statement\n- data-retention periods (including for call recordings and transcriptions)\n- encryption-at-rest\
  \ / in-transit control descriptions\n- penetration-test cadence or summary\n- incident-response or breach-notification commitment\n- uptime SLA\n- DPA availability statement\n\nevaluation_path:\n  self_serve: false\n  mechanism: >-\n    \"Customers evaluating Kixie can ask their Kixie representative which current security,\n    privacy, and contractual materials are available for their review. Availability may depend on\n    the request and applicable confidentiality requirements.\"\n  finding: >-\n    Every security artefact an enterprise buyer needs sits behind a sales conversation with an\n    explicitly conditional outcome. There is no self-serve trust portal, no NDA-gated document\n    request form, and no list of what exists — a buyer cannot even learn WHICH reports Kixie holds\n    without contacting a representative.\n\ncompliance_pointer_emitted: false\ncompliance_pointer_note: >-\n  This repo emits a `TrustCenter` pointer because the page genuinely exists and is public, but\n\
  \  emits NO `Compliance` pointer, because Kixie publishes no certification or compliance-program\n  claim. Crediting Kixie with published compliance on the strength of a routing page would be\n  exactly the kind of presence-from-absence error this pipeline exists to avoid.\n\nassessment: >-\n  As a trust centre this is thin — it is a signpost, not a disclosure. But it is an honest\n  signpost, and honest thinness is materially better than the common alternative of a badge wall\n  asserting controls that were never audited. The gap that matters most for a communications\n  platform is retention: Kixie posts call-recording URLs and AI-generated call summaries to\n  customer webhook endpoints and publishes no retention period for either.\n\ndomain_security: security/kixie-domain-security.yml\nvulnerability_disclosure: security/kixie-vulnerability-disclosure.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kixie/refs/heads/main/security/kixie-trust-center.yml
summary_line: trust center published
tags:
- Company
- Sales Engagement
- Voice
- Telephony
- SMS
- Messaging
- Contact Center
- Power Dialer
- CRM
- Webhook
- Communications
- Revenue Operations
trust_url: https://www.kixie.com/security/
---
