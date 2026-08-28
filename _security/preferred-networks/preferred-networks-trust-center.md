---
certifications:
- ISO/IEC 27001
description: Preferred Networks publishes no dedicated trust centre or trust.* subdomain, and probe-security-programs.py found neither one nor a vulnerability-disclosure programme. It does, however, publish a named certification and three downloadable governance/security policy documents from its corporate site, which are recorded here.
kind: trust-center
layout: security
name: Preferred Networks Trust Center
name_suffix: Trust Center
overview: Preferred Networks maintains a public trust center documenting ISO/IEC 27001 compliance.
provider_name: Preferred Networks
provider_slug: preferred-networks
slug: preferred-networks-trust-center
source_filename: preferred-networks-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.preferred.jp/en/company/aipolicy\nname: Preferred Networks trust, compliance and AI governance\ndescription: >-\n  Preferred Networks publishes no dedicated trust centre or trust.* subdomain, and\n  probe-security-programs.py found neither one nor a vulnerability-disclosure programme. It does,\n  however, publish a named certification and three downloadable governance/security policy documents\n  from its corporate site, which are recorded here.\ntrust_center:\n  published: false\n  probed:\n  - url: https://trust.preferred.jp/\n    status: DNS NXDOMAIN\n  note: No trust portal, subprocessor list, or downloadable audit-report request flow was found.\ncertifications:\n- name: ISO/IEC 27001\n  scope: >-\n    AI Products and Solutions Division — development, commissioned work, and provision of products\n    and services.\n  status: certified\n  statement: >-\n    \"AI Products and Solutions Division is ISO 27001-certified\
  \ for development, commissioned work and\n    provision of products and services.\"\n  source: https://www.preferred.jp/en/company/aipolicy\n  certificate_number: not published\n  auditor: not published\n  scope_note: >-\n    The certification is stated for one division, not company-wide. PFN does not publish which legal\n    entity, which registrar, or whether the PLaMo API platform falls inside the certified scope.\npolicies:\n- name: Information Security Basic Policy\n  url: http://preferred.jp/downloads/pfn_information_security_basic_policy_en.pdf\n  format: PDF\n  language: en\n- name: Cloud Security Policy\n  url: https://static.preferred.jp/downloads/pfn_cloud_security_policy_en.pdf\n  format: PDF\n  language: en\n- name: Privacy Policy\n  url: https://www.preferred.jp/en/policy/\n  format: HTML\n  language: en\nai_governance:\n  published: true\n  url: https://www.preferred.jp/en/company/aipolicy\n  framework: >-\n    An AI governance framework PFN describes as aligned with Japanese\
  \ government guidelines, under\n    management commitment, with published principles of Transparency, Risk-readiness and Integrity.\n  safety_evaluation:\n    benchmark: HELM Safety (Stanford Center for Research on Foundation Models)\n    claim: >-\n      PFN states PLaMo 3.0 Prime achieved safety performance at or above comparable overseas models\n      across HELM Safety categories, using safety data provided by NICT.\n    source: https://www.preferred.jp/ja/news/pr20260622\n    independent_verification: none published\ndata_handling:\n  zero_data_retention: >-\n    Advertised as a plan feature (ZDR — input data not retained) on the Standard and Provider plans;\n    not available on the announced Free plan.\n  training_on_customer_data: >-\n    \"Input data not used for training\" is a Standard/Provider plan feature; the Free plan does not\n    carry it.\n  data_residency: >-\n    PFN markets PLaMo as a domestic (Japanese) model; third-party coverage reports requests are\n    processed\
  \ on servers in Japan, but no first-party data-residency commitment was located in the\n    documentation, terms page (client-rendered) or product site.\n  caveat: >-\n    safety_identifier values may be persisted server-side; the API reference instructs callers not to\n    put personal or sensitive data in that field.\nvulnerability_disclosure:\n  published: false\n  security_txt: false\n  bug_bounty: none found\n  probed:\n  - url: https://www.preferred.jp/.well-known/security.txt\n    status: 404\n  - url: https://api.platform.preferredai.jp/.well-known/security.txt\n    status: 404\n  - url: https://docs.plamo.preferredai.jp/.well-known/security.txt\n    status: 404\n  note: >-\n    No security.txt, no disclosure policy page, and no HackerOne/Bugcrowd/Intigriti programme was\n    found. No Security pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preferred-networks/refs/heads/main/security/preferred-networks-trust-center.yml
summary_line: ISO/IEC 27001
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Generative AI
- LLM Inference
- Foundation Models
- Japan
- Semiconductors
- Supercomputing
- Translation
- MCP
trust_url: ''
---
