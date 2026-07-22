---
certifications: []
description: Clara operates a public Trust Center and, as a fully licensed U.S. primary care practice, is a HIPAA-covered entity. Clara publishes a HIPAA Notice of Privacy Practices and a privacy policy. No third-party security certification (SOC 2 / ISO 27001 / PCI / FedRAMP) is publicly named on the Trust Center landing page at the time of probe; the Trust Center is a JS-rendered portal and may host gated documents behind request/NDA.
kind: trust-center
layout: security
name: Clara 2 Trust Center
name_suffix: Trust Center
overview: Clara 2 maintains a public trust center covering its security and compliance posture.
provider_name: Clara 2
provider_slug: clara-2
slug: clara-2-trust-center
source_filename: clara-2-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "aid: clara-2-trust-center\nname: Clara — Trust Center & Compliance\ntype: TrustCenter\ngenerated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://trust.askclara.com (live), https://askclara.com/notice-of-privacy-practices,\n  https://askclara.com/privacy-policy\ndescription: >-\n  Clara operates a public Trust Center and, as a fully licensed U.S. primary\n  care practice, is a HIPAA-covered entity. Clara publishes a HIPAA Notice of\n  Privacy Practices and a privacy policy. No third-party security certification\n  (SOC 2 / ISO 27001 / PCI / FedRAMP) is publicly named on the Trust Center\n  landing page at the time of probe; the Trust Center is a JS-rendered portal\n  and may host gated documents behind request/NDA.\ntrust_center:\n  url: https://trust.askclara.com\n  status: 200\n  title: Clara Health Trust Center\n  gated: true\ncompliance:\n- framework: HIPAA\n  status: covered-entity\n  evidence: >-\n    Notice of Privacy Practices states \"We are required by law to\
  \ maintain the\n    privacy and security of your PHI\" and identifies \"Clara Health Medical\n    Services P.A.\" as operating under a HIPAA Organized Health Care Arrangement\n    with covered-entity affiliates.\n  source: https://askclara.com/notice-of-privacy-practices\n- framework: HSA/FSA eligibility\n  status: published\n  evidence: All subscription plans marked HSA/FSA eligible on the pricing page.\n  source: https://askclara.com/pricing\ncertifications: []\ncontacts:\n- purpose: privacy\n  email: privacy@askclara.com\n- purpose: support\n  email: support@askclara.com\nnotes: >-\n  No named SOC 2 / ISO 27001 / PCI / FedRAMP attestation is visible without\n  requesting access through the Trust Center portal. certifications[] left empty\n  rather than fabricated; revisit if Clara publishes named attestations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clara-2/refs/heads/main/security/clara-2-trust-center.yml
summary_line: trust center published
tags:
- Company
- Healthcare
- Primary Care
- Telemedicine
- Telehealth
- Artificial Intelligence
- Longevity
- Digital Health
- HIPAA
- Y Combinator
trust_url: ''
---
