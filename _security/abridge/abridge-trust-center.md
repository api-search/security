---
certifications:
- SOC 2 Type 1
- SOC 2 Type 2
- HIPAA
- CCPA
- TX-RAMP
- WCAG
description: ''
kind: trust-center
layout: security
name: Abridge Trust Center
name_suffix: Trust Center
overview: Abridge maintains a public trust center documenting SOC 2 Type 1, SOC 2 Type 2, HIPAA, CCPA, TX-RAMP, and WCAG compliance.
provider_name: Abridge
provider_slug: abridge
slug: abridge-trust-center
source_filename: abridge-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nprobe: true\nsource: https://trust.abridge.com/\nurl: https://trust.abridge.com/\nplatform: SafeBase\nplatform_note: >-\n  trust.abridge.com is a SafeBase-hosted trust portal (CNAME abridge.portals.safebase.io).\n  The content — certifications, controls, subprocessors, document library — is Abridge's;\n  the /.well-known/ OAuth documents served on that host are SafeBase's and are recorded as\n  vendor-owned in well-known/abridge-well-known.yml.\naccess: public\ncertifications:\n  - name: SOC 2 Type 1\n    status: certified\n  - name: SOC 2 Type 2\n    status: certified\n  - name: HIPAA\n    status: compliant\n  - name: CCPA\n    status: compliant\n  - name: TX-RAMP\n    status: certified\n  - name: WCAG\n    status: conformant\ndocuments:\n  - name: SOC 2 Report\n    access: on-request\n  - name: Security Whitepaper\n    access: on-request\n  - name: Network Diagram\n    access: on-request\n  - name: Business Continuity / Disaster\
  \ Recovery Policy\n    access: on-request\ncontrols:\n  - Audit logging\n  - Data security\n  - Multi-factor authentication\n  - Application penetration testing\n  - Network penetration testing\n  - Code analysis\n  - Secure development training\n  - AI training data and bias assessment\n  - AI security\n  - AI monitoring\n  - Access monitoring\n  - Certificates of destruction\n  - Data asset classification\n  - Anti-DDoS\n  - Anti-malware\n  - Disk encryption\n  - Endpoint detection and response\n  - Firewall\n  - Security information and event management (SIEM)\n  - Vulnerability and patch management\n  - Employee security training\nsubprocessors:\n  - Google Cloud\n  - OpenAI\n  - Zendesk\n  - Amplitude\n  - Sentry\nvulnerability_disclosure:\n  published: false\n  note: >-\n    The trust center describes an internal vulnerability and patch management program but\n    publishes no public reporting channel, responsible-disclosure policy or bug bounty.\n    https://www.abridge.com/security,\
  \ /trust, /responsible-disclosure and\n    /vulnerability-disclosure all return 404; hackerone.com/abridge and bugcrowd.com/abridge\n    both return 404; no Abridge-served security.txt exists (see well-known/).\nevidence:\n  - source: https://trust.abridge.com/\n    http_status: 200\n    keywords:\n      - soc 2 type 1\n      - soc 2 type 2\n      - hipaa\n      - ccpa\n      - tx-ramp\n      - wcag\n      - penetration testing\n      - subprocessors\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abridge/refs/heads/main/security/abridge-trust-center.yml
summary_line: SOC 2 Type 1, SOC 2 Type 2, HIPAA, CCPA, TX-RAMP, WCAG
tags:
- Healthcare
- Ambient AI
- Clinical Documentation
- Generative AI
- Revenue Cycle
- Nursing Documentation
- EHR Integration
- Epic
trust_url: https://trust.abridge.com/
---
