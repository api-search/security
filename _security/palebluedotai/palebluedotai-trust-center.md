---
certifications:
- ISO/IEC 27001
- SOC 2
- SOC 3
description: ''
kind: trust-center
layout: security
name: Palebluedotai Trust Center
name_suffix: Trust Center
overview: PaleBlueDot.AI maintains a public trust center documenting ISO/IEC 27001, SOC 2, and SOC 3 compliance.
provider_name: PaleBlueDot.AI
provider_slug: palebluedotai
slug: palebluedotai-trust-center
source_filename: palebluedotai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.palebluedot.ai/about/\nurl: https://www.palebluedot.ai/about/\nname: PaleBlueDot.AI security and compliance\npage_title: Security & Compliance (section of the About Us page)\ncorrected_url_note: >-\n  An automated probe initially recorded this artifact at https://www.palebluedot.ai/trust.\n  THAT URL IS A SOFT 404 and has been corrected. Verified 2026-08-26: /trust returns HTTP 200\n  with a body byte-identical to the homepage (49129 bytes), the title \"PaleBlueDot AI - The\n  Intelligence Platform\" and rel=canonical pointing at \"/\". The Astro site answers 200 with the\n  homepage for every unknown path, and the homepage itself contains the compliance keywords, so a\n  keyword probe scores a hit on a page that does not exist. The real surface is the Security &\n  Compliance section of the About Us page.\ncertifications:\n- name: ISO/IEC 27001\n  holder: Digital Realty\n  scope: Physical infrastructure and facility\
  \ operations of the colocation data centres\n  held_by_provider: false\n- name: SOC 2\n  holder: Digital Realty\n  scope: Physical infrastructure and facility operations of the colocation data centres\n  held_by_provider: false\n- name: SOC 3\n  holder: Digital Realty\n  scope: Physical infrastructure and facility operations of the colocation data centres\n  held_by_provider: false\nattribution_warning: >-\n  READ THIS BEFORE CITING THE CERTIFICATIONS. None of the certifications above belong to\n  PaleBlueDot AI. The company's own wording is explicit: \"Data Center & Facility Compliance\n  (Provided by Digital Realty) - Our primary colocation facilities are provided by Digital Realty.\n  These facilities are certified and maintained under the ISO/IEC 27001 Information Security\n  Management System, and backed by SOC 2 / SOC 3 reports covering physical infrastructure and\n  facility operations.\" These are the LANDLORD'S facility certifications, inherited by tenancy.\n  No company-level,\
  \ platform-level or software-level audit of PaleBlueDot AI or of the TokenRouter\n  gateway is claimed or published. Recording these as PaleBlueDot certifications would be a\n  misattribution of the same class the catalogue has been burned by before.\nverification_documents:\n  publicly_available: false\n  process: >-\n    \"Verification documents can be made available upon request. For security reasons, we can\n    facilitate access to these materials through our data center provider upon signing an NDA.\"\n  gate: NDA, and routed through the data centre provider rather than the company.\nprovider_stated_commitments:\n- claim: Security and trust come first; platform and operational controls are continually strengthened to provide verifiable protection for enterprise customers.\n  audited: false\n  source: https://www.palebluedot.ai/about/\n- claim: Zero Data Retention (ZDR) - only request metadata is logged; prompts and completions are never stored.\n  audited: false\n  source: https://www.tokenrouter.com/docs/faq/\n\
  \  note: A significant and specific commitment, but self-asserted - no third-party attestation of it is published.\ndata_processing:\n  dpa_published: true\n  dpa_url: https://www.tokenrouter.com/docs/global-dpa/\n  dpa_title: TOKENROUTER - GLOBAL DATA PROCESSING AGREEMENT\n  http_status: 200\n  note: A published global DPA is a genuine and uncommon compliance artifact for a company at this stage.\nvulnerability_disclosure:\n  published: false\n  bug_bounty: false\n  security_txt: false\n  security_contact: null\n  note: >-\n    PROBED 2026-08-26 - no security.txt on any of the four hosts, no disclosure policy page, and no\n    HackerOne/Bugcrowd/Intigriti programme found. The only published contact is the general\n    support@tokenrouter.com address. No type Security pointer is emitted in apis.yml, because there\n    is no disclosure programme to point at.\n  cross_ref: security/palebluedotai-vulnerability-disclosure.yml (not written - nothing to record)\nx-evidence:\n- url: https://www.palebluedot.ai/about/\n\
  \  http_status: 200\n  fetched: '2026-08-26'\n- url: https://www.palebluedot.ai/trust\n  http_status: 200\n  served: false\n  note: Soft 404 - byte-identical to the homepage, canonical \"/\". Rejected.\n  fetched: '2026-08-26'\n- url: https://www.tokenrouter.com/docs/global-dpa/\n  http_status: 200\n  fetched: '2026-08-26'\n- url: https://www.tokenrouter.com/docs/faq/\n  http_status: 200\n  fetched: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palebluedotai/refs/heads/main/security/palebluedotai-trust-center.yml
summary_line: ISO/IEC 27001, SOC 2, SOC 3
tags:
- Artificial Intelligence
- Machine-Learning
- Large Language Models
- Inference
- API Gateway
- GPU
- Cloud Computing
- Model Routing
- Compute
- Company
trust_url: https://www.palebluedot.ai/about/
---
