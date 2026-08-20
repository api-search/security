---
api_specs:
- filename: healthie-webhooks-asyncapi.yml
  format: yaml
  label: Healthie GraphQL API
  slug: healthie-graphql-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthie/refs/heads/main/asyncapi/healthie-webhooks-asyncapi.yml
certifications:
- HIPAA
- SOC 2 Type 2
- HITRUST CSF r2
- ONC Health IT Certification
- PCI DSS Service Provider Level 1 (held by Healthie's payment processor, not by Healthie)
- GDPR
- PIPEDA
description: ''
kind: trust-center
layout: security
name: Healthie Trust Center
name_suffix: Trust Center
overview: Healthie maintains a public trust center documenting HIPAA, SOC 2 Type 2, HITRUST CSF r2, ONC Health IT Certification, PCI DSS Service Provider Level 1 (held by Healthie's payment processor, not by Healthie), GDPR, and PIPEDA compliance.
provider_name: Healthie
provider_slug: healthie
slug: healthie-trust-center
source_filename: healthie-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://trust.gethealthie.com\nurl: https://trust.gethealthie.com\nplatform: Vanta\nplatform_evidence: 'og:image resolves to https://app.vanta.com/doc?s=7fl6tpu48qh2pynckbhde'\nrendering: javascript-rendered\nrendering_note: >-\n  The trust center returns HTTP 200 but its served HTML is an empty shell — the certification list,\n  document requests and subprocessor table only exist after script execution. The certification list\n  below was therefore read from the server-rendered security page at\n  https://www.gethealthie.com/security, which enumerates the same programs in crawlable HTML.\nsecondary_source: https://www.gethealthie.com/security\ncertifications:\n- HIPAA\n- SOC 2 Type 2\n- HITRUST CSF r2\n- ONC Health IT Certification\n- PCI DSS Service Provider Level 1 (held by Healthie's payment processor, not by Healthie)\n- GDPR\n- PIPEDA\nbaa:\n  available: true\n  url: https://www.gethealthie.com/baa\nsecurity_program:\n\
  - Annual third-party penetration testing\n- Annual disaster recovery tabletop exercises\n- Annual risk assessments\n- Quarterly vulnerability scans\n- Biometric access control, surveillance and 24/7 guards at hosting facilities\n- Redundant power and data backup under a documented disaster recovery plan\n- 256-bit TLS for data in transit\n- Audit logging across application, SQL query and platform backend activity\ncyber_insurance:\n  published: true\n  note: >-\n    Healthie publishes a cybersecurity coverage article covering technology and professional\n    liability, security and privacy liability and security breach response.\n  url: https://help.gethealthie.com/article/1114-cybersecurity-coverage\ncontacts:\n  compliance: compliance@gethealthie.com\n  general: hello@gethealthie.com\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No vulnerability disclosure program was found. There is no /.well-known/security.txt on any\n    Healthie host, no /responsible-disclosure\
  \ or /vulnerability-disclosure page, and no HackerOne or\n    Bugcrowd program (hackerone.com/healthie and bugcrowd.com/healthie both 404). Healthie publishes\n    a compliance@ address but no security-reporting address and no safe-harbour statement. For a\n    HITRUST- and SOC 2-certified platform holding PHI, this is the most conspicuous single gap on the\n    public security surface — and the cheapest to close. No VulnerabilityDisclosure or Security\n    pointer is wired into apis.yml, because there is nothing to point at.\n  checked: '2026-08-14'\nsupersedes:\n  previous_source: https://www.gethealthie.com/hipaa-compliant-software\n  previous_certifications: [HIPAA, GDPR]\n  reason: >-\n    The automated probe (0-working/probe-security-programs.py) matched a marketing page carrying only\n    two keywords. This pass replaces it with the actual Vanta trust center plus the full\n    server-rendered certification list.\nevidence:\n- {source: 'https://trust.gethealthie.com', http_status:\
  \ 200, keywords: [trust center, security,\n      compliance]}\n- {source: 'https://www.gethealthie.com/security', http_status: 200, keywords: [hipaa, soc 2, hitrust,\n      onc, pci, gdpr, pipeda]}\n- {source: 'https://www.gethealthie.com/baa', http_status: 200, keywords: [business associate agreement]}\n- {source: 'https://hackerone.com/healthie', http_status: 404}\n- {source: 'https://bugcrowd.com/healthie', http_status: 404}\n- {source: 'https://www.gethealthie.com/.well-known/security.txt', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthie/refs/heads/main/security/healthie-trust-center.yml
summary_line: HIPAA, SOC 2 Type 2, HITRUST CSF r2, ONC Health IT Certification, PCI DSS Service Provider Level 1 (held by Healthie's payment processor, not by Healthie), GDPR, PIPEDA
tags:
- API-First
- Appointments
- Billing
- Care Plans
- Charting
- Claims
- Clinical
- Digital Health
- EHR
- EMR
- Forms
- GraphQL
- Health Tech
- Healthcare
- Insurance
- Intake
- Online Programs
- Patient Engagement
- Patient Portal
- Practice Management
- Programs
- Scheduling
- Telehealth
- Wellness
- Webhook
trust_url: https://trust.gethealthie.com
---
