---
certifications:
- SOC 2
- SOC 3
description: ''
kind: trust-center
layout: security
name: Merlyn Mind Trust Center
name_suffix: Trust Center
overview: Merlyn Mind maintains a public trust center documenting SOC 2 and SOC 3 compliance.
provider_name: Merlyn Mind
provider_slug: merlyn-mind
slug: merlyn-mind-trust-center
source_filename: merlyn-mind-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nprobe: true\nsource: https://trust.merlyn.org/\nurl: https://trust.merlyn.org/\nplatform: SafeBase by Drata\nnote: >-\n  trust.merlyn.org is a SafeBase (Drata) hosted trust center. It answers our crawler with a\n  Cloudflare interstitial (HTTP 403, \"Just a moment...\"), so the page is LIVE but bot-challenged;\n  the contents below were read through a browser-agent fetch of the same URL. Some documents\n  (SOC 2 report, pentest report, network diagram) are gated behind an NDA/request flow typical of\n  SafeBase; the certification list and the security contact are public on the landing page.\ncertifications:\n- SOC 2\n- SOC 3\nregulatory_frameworks:\n- COPPA\n- FERPA\n- GDPR\ndocuments:\n- name: SOC 2 Report\n  access: request/NDA\n- name: Pentest Report\n  access: request/NDA\n- name: Network Diagram\n  access: request/NDA\n- name: Merlyn Security Flyer\n  access: request/NDA\n- name: Merlyn Privacy Flyer\n  access: request/NDA\nsubprocessors:\n\
  - Amazon\n- Google Cloud\n- Microsoft\n- Salesforce\nsecurity_contact: security@merlyn.org\nproduct_security:\n- multi-factor authentication\n- single sign-on (SSO)\nevidence:\n- source: https://trust.merlyn.org/\n  http_status: 403\n  note: >-\n    Cloudflare bot challenge to the raw crawler; page demonstrably exists and renders for a\n    browser agent. Certifications, subprocessors, document list and security contact read from\n    that render.\n  keywords:\n  - soc 2\n  - soc 3\n  - coppa\n  - ferpa\n  - gdpr\n  - trust center\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merlyn-mind/refs/heads/main/security/merlyn-mind-trust-center.yml
summary_line: SOC 2, SOC 3
tags:
- Company
- Artificial Intelligence
- Education
- EdTech
- K-12
- Large Language Models
- Voice Assistant
- Classroom Technology
- Machine-Learning
- Responsible AI
trust_url: https://trust.merlyn.org/
---
