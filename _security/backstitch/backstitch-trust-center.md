---
certifications:
- SOC for Service Organizations (AICPA)
description: ''
kind: trust-center
layout: security
name: Backstitch Trust Center
name_suffix: Trust Center
overview: backstitch maintains a public trust center documenting SOC for Service Organizations (AICPA) compliance.
provider_name: backstitch
provider_slug: backstitch
slug: backstitch-trust-center
source_filename: backstitch-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://trust.backstitch.io/\ntrust_center:\n  url: https://trust.backstitch.io/\n  status: 200\n  title: backstitch Trust Center\n  platform: Vanta\n  platform_evidence: >-\n    The served HTML is a Vanta trust-report shell — assets.vanta.com static\n    bundle, data-environment=\"prod\", data-slugid=\"h77c0lxbsolmn6ttdutbtv\",\n    stylesheet index-trust-report-*.css.\n  linked_from:\n    - label: Security & Compliance (site nav/footer)\n      url: https://www.backstitch.io/\n  description: >-\n    \"backstitch is committed protecting your data with robust practices,\n    certifications, and industry leading safeguards. Review our policies and\n    certifications, and see how backstitch is a service you can trust.\" (verbatim\n    meta description of https://trust.backstitch.io/)\ncertifications:\n- name: SOC for Service Organizations (AICPA)\n  status: claimed\n  report_type: null\n  period: null\n  auditor: null\n  evidence:\
  \ >-\n    AICPA SOC non-CPA badge published on the backstitch homepage\n    (https://www.backstitch.io/hs-fs/hubfs/21972-312_SOC_NonCPA.png) linking to\n    http://www.aicpa.org/soc4so. The badge asserts a SOC examination; backstitch\n    does not state Type I vs Type II, the audit period, or the auditing firm on\n    any anonymously readable page.\nreadability:\n  machine_readable: false\n  note: >-\n    The trust center's substance — control list, certification records, document\n    downloads — is rendered client-side by the Vanta bundle and is not present in\n    the served HTML. The Vanta data API refuses anonymous reads\n    (https://api.vanta.com/v1/public/trust-report/h77c0lxbsolmn6ttdutbtv -> 401;\n    the legacy https://api.vanta.com/graphql -> 410 Gone), so the certification\n    list could not be enumerated without a request-access flow. Only the SOC\n    badge on backstitch's own homepage is independently verifiable.\n  spa_catch_all_warning: >-\n    trust.backstitch.io answers\
  \ HTTP 200 with the same SPA shell for EVERY path,\n    including /.well-known/agent-card.json, /.well-known/security.txt,\n    /robots.txt and /sitemap.xml. Those 200s are not documents and must not be\n    read as discovery hits. See well-known/backstitch-well-known.yml.\nprobes:\n- url: https://trust.backstitch.io/\n  status: 200\n- url: https://api.vanta.com/v1/public/trust-report/h77c0lxbsolmn6ttdutbtv\n  status: 401\n- url: https://api.vanta.com/graphql\n  status: 410\n- url: https://www.backstitch.io/\n  status: 200\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backstitch/refs/heads/main/security/backstitch-trust-center.yml
summary_line: SOC for Service Organizations (AICPA)
tags:
- Company
- Content Curation
- Employee Communications
- Internal Communications
- Total Rewards
- Content Aggregation
- Newsletters
- Widgets
- REST
trust_url: ''
---
