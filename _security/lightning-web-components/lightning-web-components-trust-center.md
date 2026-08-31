---
certifications:
- PCI DSS
- IRAP
description: Trust and compliance surface applicable to Lightning Web Components. LWC OSS is a library and operates no service of its own, so it holds no certifications directly. The operative trust surface for components running on the Salesforce Platform is the parent brand's, recorded here with that scope stated explicitly rather than claimed as an LWC certification.
kind: trust-center
layout: security
name: Lightning Web Components Trust Center
name_suffix: Trust Center
overview: Lightning Web Components maintains a public trust center documenting PCI DSS and IRAP compliance.
provider_name: Lightning Web Components
provider_slug: lightning-web-components
slug: lightning-web-components-trust-center
source_filename: lightning-web-components-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://trust.salesforce.com/\nprovider: Lightning Web Components\nproviderId: lightning-web-components\ndescription: >-\n  Trust and compliance surface applicable to Lightning Web Components. LWC OSS is a library and\n  operates no service of its own, so it holds no certifications directly. The operative trust\n  surface for components running on the Salesforce Platform is the parent brand's, recorded here\n  with that scope stated explicitly rather than claimed as an LWC certification.\nscope: parent-brand\nparent: Salesforce\ntrust_center:\n  url: https://trust.salesforce.com/\n  status: 200\n  status_page: https://status.salesforce.com/\n  status_page_status: 200\ncompliance_portal:\n  url: https://compliance.salesforce.com/\n  status: 200\n  documents_url: https://compliance.salesforce.com/en/documents\n  documents_status: 200\n  statement: '\"Salesforce maintains a comprehensive set of compliance certifications and attestations.\"\
  '\n  document_count_reported: 505\ncertifications:\n  - name: PCI DSS\n    evidence: PCI ASV Network Scan documents listed across Hyperforce regions and first-party infrastructure at https://compliance.salesforce.com/en/documents\n  - name: IRAP\n    evidence: ACSC Essential 8 report (IRAP assessment) listed at https://compliance.salesforce.com/en/documents\ncompleteness_note: >-\n  The compliance document library reports 505 entries and paginates ten at a time; only the first\n  page was read in this pass. The two certifications above are the ones actually observed. SOC,\n  ISO 27001 and FedRAMP were NOT enumerated here and are deliberately not asserted — an honest\n  partial reading rather than a guessed list.\nlwc_specific:\n  certifications: []\n  note: >-\n    The Lightning Web Components open-source project itself publishes no certification, audit\n    report or trust page. Its security posture is expressed as a minimal-runtime-dependency policy\n    plus the SECURITY.md reporting\
  \ channel — see\n    security/lightning-web-components-vulnerability-disclosure.yml.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightning-web-components/refs/heads/main/security/lightning-web-components-trust-center.yml
summary_line: PCI DSS, IRAP
tags:
- Frontend
- JavaScript
- Lightning Web Components
- Salesforce
- Web Components
- Custom Elements
- Shadow DOM
- Open Source
- UI Framework
- Component Library
trust_url: ''
---
