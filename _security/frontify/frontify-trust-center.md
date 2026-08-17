---
certifications:
- SOC 2 Type II
- ISO 27001:2022
- Cyber Essentials
- TISAX
- Swiss-US Data Privacy Framework
- GDPR
- PCI
- HIPAA
description: Frontify runs its trust center on Conveyor. The page is JS-rendered, but the bootstrap payload embeds Frontify's own canonical vendor record, which is where the certification list below comes from — read out of the record whose "website" field is http://www.frontify.com, not off the rendered page.
kind: trust-center
layout: security
name: Frontify Trust Center
name_suffix: Trust Center
overview: Frontify maintains a public trust center documenting SOC 2 Type II, ISO 27001:2022, Cyber Essentials, TISAX, Swiss-US Data Privacy Framework, GDPR, PCI, and HIPAA compliance.
provider_name: Frontify
provider_slug: frontify
slug: frontify-trust-center
source_filename: frontify-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nprobe: true\nsource: https://trust.frontify.com/\nurl: https://trust.frontify.com/\nplatform: Conveyor\ndataroom: https://app.conveyor.com/datarooms/d6f77cab-a507-48af-bfb9-771eddc3f398\ndescription: >-\n  Frontify runs its trust center on Conveyor. The page is JS-rendered, but the bootstrap\n  payload embeds Frontify's own canonical vendor record, which is where the certification\n  list below comes from — read out of the record whose \"website\" field is\n  http://www.frontify.com, not off the rendered page.\ncertifications:\n  - SOC 2 Type II\n  - ISO 27001:2022\n  - Cyber Essentials\n  - TISAX\n  - Swiss-US Data Privacy Framework\n  - GDPR\n  - PCI\n  - HIPAA\ncertification_ids_verbatim:\n  - soc2-type-2\n  - iso-27001-2022\n  - cyber-essentials\n  - tisax\n  - swiss-us-dpf\n  - gdpr\n  - pci\n  - hipaa\nsoc2:\n  status: first SOC 2 Type II examination completed\n  announced: '2026-07-07'\n  report_access: available on request through\
  \ the Trust Center\n  quote: >-\n    \"We're pleased to share that Frontify has successfully completed its first SOC 2\n    Type II examination... This milestone marks the beginning of our ongoing SOC 2\n    program. As part of our commitment to continuous improvement, future SOC 2 Type II\n    examinations will cover a longer observation period and an expanded scope.\"\n  note: >-\n    Worth reading precisely: this is Frontify's FIRST Type II, announced 2026-07-07, with\n    a deliberately narrow first observation period. It is a real attestation, not a\n    long-running program.\nsecurity_qa:\n  published: true\n  note: >-\n    Frontify announced a Security Q&A section in the trust center covering frequently\n    asked security questions on policies, certifications and procedures.\ncorrection:\n  applied: '2026-08-13'\n  previous_claim: [SOC 2, ISO 27001, ISO 27017, ISO 27018, HIPAA, FedRAMP, GDPR, CSA STAR]\n  what_was_wrong: >-\n    The previous round credited Frontify with ISO 27017,\
  \ ISO 27018, FedRAMP and CSA STAR.\n    NONE of those belong to Frontify. The trust.frontify.com bootstrap payload also\n    embeds OTHER vendors' Conveyor records — Datadog (iso-27017, iso-27018,\n    fedramp-li-saas), Splunk (fedramp-moderate, CSA STAR 2) and AWS (fedramp, csa) — and\n    a keyword scan of the page body cannot tell whose certification it just matched. The\n    earlier artifact matched on the page, not on Frontify's record.\n  what_was_missed: >-\n    The same error dropped four certifications Frontify genuinely holds — Cyber\n    Essentials, TISAX, Swiss-US DPF and PCI — and lost the ISO 27001 vintage (2022).\n  rule: >-\n    On a shared trust-center platform (Conveyor, SafeBase, Vanta, Drata), match the\n    vendor record by its own website/slug field before reading any certification list.\n    A keyword hit on the page is not evidence about this company.\nevidence:\n  - source: https://trust.frontify.com/\n    http_status: 200\n    kind: trust-center\n    matched_record:\
  \ 'canonical_asset/vendor \"Frontify\", slug \"frontify\", website http://www.frontify.com'\n    checked: '2026-08-13'\nrelated:\n  security_page: https://www.frontify.com/en/security/\n  vulnerability_disclosure: security/frontify-vulnerability-disclosure.yml\n  legal:\n    - https://www.frontify.com/en/legal/data-processing-agreement\n    - https://www.frontify.com/en/legal/technical-and-organizational-measures\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontify/refs/heads/main/security/frontify-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001:2022, Cyber Essentials, TISAX, Swiss-US Data Privacy Framework, GDPR, PCI, HIPAA
tags:
- Company
- Marketing
- Brand Management
- Digital Asset Management
- DAM
- Content
- GraphQL
- Creative Operations
trust_url: https://trust.frontify.com/
---
