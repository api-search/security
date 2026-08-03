---
certifications:
- ioXt Alliance certification
- Google MASA (Mobile Application Security Assessment)
- UL / FCC / Energy Star
description: ''
kind: trust-center
layout: security
name: Wyze Trust Center
name_suffix: Trust Center
overview: Wyze maintains a public trust center documenting ioXt Alliance certification, Google MASA (Mobile Application Security Assessment), and UL / FCC / Energy Star compliance.
provider_name: Wyze
provider_slug: wyze
slug: wyze-trust-center
source_filename: wyze-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nurl: https://www.wyze.com/pages/security-trust\ntitle: Wyze security\nnotes: >-\n  Wyze operates a public security/trust hub rather than a vendor trust portal (no\n  SafeBase/Vanta-style document request flow, no downloadable audit reports). It names\n  device- and app-level certifications and third-party testing rather than enterprise\n  attestations. IMPORTANT ATTRIBUTION: the page cites \"Using AWS infrastructure (SOC2 &\n  ISO compliance)\" - that is the compliance posture of Wyze's cloud PROVIDER, not a Wyze\n  attestation. Wyze does not publish a SOC 2 report, ISO 27001 certificate, PCI DSS AOC,\n  HIPAA or FedRAMP status of its own, and none is claimed here.\ncertifications:\n- name: ioXt Alliance certification\n  scope: Wyze iOS & Android apps\n  note: Wyze describes ioXt as the leading connected-device security certification.\n- name: Google MASA (Mobile Application Security Assessment)\n  scope: Android app\n\
  - name: UL / FCC / Energy Star\n  scope: specific hardware lines (e.g. light bulbs)\nthird_party_testing:\n- provider: NCC Group\n  activity: penetration testing (passed)\n- provider: ReFirm Labs\n  activity: third-party hardware security testing (passed)\n- provider: Bitdefender\n  activity: in-depth penetration testing of Wyze Cam v3\ninherited_infrastructure_compliance:\n- provider: Amazon Web Services\n  claims: [SOC 2, ISO]\n  attributed_to: AWS, not Wyze\nsecurity_controls_published:\n- mandatory 2-factor authentication for all customers\n- Lacework deployed for cloud infrastructure security\n- AWS WAF and Amazon GuardDuty in use\n- VerifiedView - a hashed user ID embedded into every video, photo and livestream so only\n  the rightful account owner can access the content\n- live stream and video encryption between mobile device, Wyze product and AWS cloud\nprivacy_position: >-\n  Wyze states it does not sell personal information for money, while disclosing that\n  sharing certain\
  \ activity data with advertising and business partners may constitute a\n  \"sale\" under CCPA and similar state privacy laws.\nrelated_pages:\n  privacy_policy: https://www.wyze.com/policies/privacy-policy\n  terms_of_service: https://www.wyze.com/policies/terms-of-service\n  vulnerability_disclosure: https://www.wyze.com/pages/wyzes-vulnerability-disclosure\n  suspicious_activity: https://www.wyze.com/pages/security-report\n  security_transparency_report: https://www.wyze.com/pages/response-to-3-29-22-security-report\nevidence:\n- source: https://www.wyze.com/pages/security-trust\n  http_status: 200\n  keywords: [security, trust, ioXt, Google MASA, penetration testing, SOC2, ISO, 2-factor]\nx-evidence:\n  fetched: '2026-08-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyze/refs/heads/main/security/wyze-trust-center.yml
summary_line: ioXt Alliance certification, Google MASA (Mobile Application Security Assessment), UL / FCC / Energy Star
tags:
- Company
- Smart Home
- Internet of Things
- Home Security
- Cameras
- Consumer Electronics
- Home Automation
- Video
- Sensors
- Commerce
trust_url: https://www.wyze.com/pages/security-trust
---
