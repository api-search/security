---
certifications:
- SOC 2 Type II
- GDPR
description: AnnounceKit's trust posture. SOC 2 Type II and GDPR are both claimed on the provider's own trust page, with an independently verified security report published through Drata. Upgraded 2026-09-02 from a keyword-match record to the named program detail on https://announcekit.app/trust and https://announcekit.app/security.
kind: trust-center
layout: security
name: Announcekit Trust Center
name_suffix: Trust Center
overview: AnnounceKit maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: AnnounceKit
provider_slug: announcekit
slug: announcekit-trust-center
source_filename: announcekit-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nprobe: true\nsource: https://announcekit.app/trust\nurl: https://announcekit.app/trust\nprovider: AnnounceKit\nproviderId: announcekit\ndescription: >-\n  AnnounceKit's trust posture. SOC 2 Type II and GDPR are both claimed on the\n  provider's own trust page, with an independently verified security report\n  published through Drata. Upgraded 2026-09-02 from a keyword-match record to\n  the named program detail on https://announcekit.app/trust and\n  https://announcekit.app/security.\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n  scope: Security, Availability, and Confidentiality\n  auditor: Independently verified by a licensed CPA firm\n  report_availability: >-\n    Available to Enterprise customers who have signed an NDA. Requested through\n    an account executive or support@announcekit.app.\n  source: https://announcekit.app/trust\n- name: GDPR\n  status: compliant\n  detail: >-\n    Data processing agreement\
  \ available, data portability supported, deletion\n    requests honored.\n  source: https://announcekit.app/gdpr-compliance\ntrust_center:\n  platform: Drata\n  name: Drata Trust Center\n  linked_from: https://announcekit.app/trust\n  note: >-\n    AnnounceKit links out to a Drata-hosted security profile carrying compliance\n    status, controls and audit history, rather than hosting the evidence itself.\ndocuments:\n- {name: Data Processing Agreement, linked_from: 'https://announcekit.app/trust'}\n- {name: Privacy Policy, url: 'https://announcekit.app/privacy-policy', status: 200}\n- {name: Terms of Service, url: 'https://announcekit.app/terms-of-service', status: 200}\n- {name: Cookie Policy, linked_from: 'https://announcekit.app/trust'}\n- {name: Security Overview, url: 'https://announcekit.app/security', status: 200}\n- {name: SOC 2 page, url: 'https://announcekit.app/soc2', status: 200}\n- {name: GDPR Compliance, url: 'https://announcekit.app/gdpr-compliance', status: 200}\ncontrols:\n\
  \  infrastructure: Amazon Web Services, SOC 2 compliant providers\n  encryption_at_rest: AES-256\n  encryption_in_transit: 256-bit HTTPS; TLS 1.0 and 1.1 support ended (announced 2026-04-21)\n  payment_data: No direct access; handled by Stripe\n  access_control: [SAML 2.0 SSO, TOTP two-factor, RBAC (owner/manager/editor/viewer),\n    IP access control, audit log]\n  operational: [Automated software scanning and vulnerability remediation, Regular penetration\n    testing, SOC 2 incident response plan with a dedicated security team]\n  observed_headers:\n    url: https://announcekit.app/gq/v2\n    Strict-Transport-Security: max-age=31536000\n    X-Content-Type-Options: nosniff\n    Referrer-Policy: strict-origin-when-cross-origin\n    fetched: '2026-09-02'\nevidence:\n- source: https://announcekit.app/trust\n  http_status: 200\n  keywords: [soc 2 type ii, gdpr, dpa, drata, trust center]\n- source: https://announcekit.app/security\n  http_status: 200\n  keywords: [aes-256, penetration testing,\
  \ saml sso, rbac, 2fa, ip access control, audit log]\ngaps:\n- >-\n  No public vulnerability disclosure program. No security.txt on\n  announcekit.app (404), no bug bounty on HackerOne, Bugcrowd or Intigriti, and\n  no disclosure policy page. The security page names penetration testing and an\n  incident response plan but gives a researcher no channel to report into.\n- >-\n  The SOC 2 report is gated behind an Enterprise contract plus an NDA, so the\n  certification cannot be independently verified from the public surface.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/announcekit/refs/heads/main/security/announcekit-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Changelog
- Feature Requests
- NPS
- Notification
- Product Communication
- Roadmaps
- Software-as-a-Service
- Widgets
trust_url: https://announcekit.app/trust
---
