---
certifications:
- SOC 2 Type 2
- ISO/IEC 27001:2022
- ISO/IEC 27017:2015
- ISO/IEC 27018:2019
- ISO/IEC 27701:2019
- PCI DSS v4.0.1
- HIPAA
- GDPR
- FIPS 140-2
- FIPS 140-3
- CASA Tier 2
- NIST CSF
- EU AI Act
description: ''
kind: trust-center
layout: security
name: Uniphore Trust Center
name_suffix: Trust Center
overview: Uniphore maintains a public trust center documenting SOC 2 Type 2, ISO/IEC 27001:2022, ISO/IEC 27017:2015, ISO/IEC 27018:2019, ISO/IEC 27701:2019, PCI DSS v4.0.1, HIPAA, GDPR, FIPS 140-2, FIPS 140-3, CASA Tier 2, NIST CSF, and EU AI Act compliance.
provider_name: Uniphore
provider_slug: uniphore
slug: uniphore-trust-center
source_filename: uniphore-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nsource: https://trust.uniphore.com/\nurl: https://trust.uniphore.com/\nplatform: SafeBase (uniphore.portals.safebase.io)\ncontact: uniphore_trust@uniphore.com\ncertifications:\n- SOC 2 Type 2\n- ISO/IEC 27001:2022\n- ISO/IEC 27017:2015\n- ISO/IEC 27018:2019\n- ISO/IEC 27701:2019\n- PCI DSS v4.0.1\n- HIPAA\n- GDPR\n- FIPS 140-2\n- FIPS 140-3\n- CASA Tier 2\n- NIST CSF\n- EU AI Act\ndocuments:\n- Compliance attestations (SOC 2, ISO, HIPAA, PCI DSS, CASA Tier 2)\n- Penetration testing reports\n- Data Processing Agreement\n- Privacy Policy\n- Access Control Policy\n- Cyber Insurance certificate\n- W-9\nsecondary_sources:\n- url: https://www.uniphore.com/security/\n  certifications_named:\n  - ISO/IEC 27001:2022\n  - PCI DSS (Level 1 Service Provider)\n  - SOC 2 Type II\n- url: https://www.uniphore.com/legal/dpa/\n  kind: data-processing-agreement\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No published\
  \ vulnerability disclosure or bug bounty program was found.\n    /.well-known/security.txt is 404 on every Uniphore host; hackerone.com/uniphore\n    and bugcrowd.com/uniphore both 404; no /responsible-disclosure or\n    /vulnerability-disclosure page exists on uniphore.com. The Trust Center does\n    publish penetration testing reports and a uniphore_trust@uniphore.com contact,\n    but neither constitutes a disclosure policy. No Security /\n    VulnerabilityDisclosure pointer is emitted for this provider.\nevidence:\n- source: DNS\n  detail: trust.uniphore.com CNAME uniphore.portals.safebase.io\n- source: https://trust.uniphore.com/\n  keywords:\n  - soc 2\n  - iso/iec 27001\n  - iso/iec 27017\n  - iso/iec 27018\n  - pci dss\n  - hipaa\n  - gdpr\n  - fips 140\n  - trust center\n  - penetration testing\n- source: https://www.uniphore.com/security/\n  keywords:\n  - iso 27001\n  - pci dss\n  - soc2 type ii\nx-evidence:\n- url: https://trust.uniphore.com/\n  http_status: 403\n  note: >-\n\
  \    Direct curl hits a Cloudflare interstitial; content confirmed on 2026-08-02 by\n    a rendering fetch and independently by 0-working/probe-security-programs.py,\n    which matched trust/compliance keywords in the body.\n  fetched: '2026-08-02'\n- url: https://www.uniphore.com/security/\n  http_status: 200\n  fetched: '2026-08-02'\n- url: https://hackerone.com/uniphore\n  http_status: 404\n  fetched: '2026-08-02'\n- url: https://bugcrowd.com/uniphore\n  http_status: 404\n  fetched: '2026-08-02'\n- url: https://trust.uniphore.com/\n  http_status: 200\n  note: >-\n    Re-verified 2026-08-14 by 0-working/probe-security-programs.py, which again\n    matched SOC 2, ISO 27001/27017/27018, PCI DSS, HIPAA, GDPR and FIPS 140 in the\n    body. The probe's own output is a keyword-level subset of the certification\n    list captured on 2026-08-02; the richer searched version above is retained.\n  fetched: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniphore/refs/heads/main/security/uniphore-trust-center.yml
summary_line: SOC 2 Type 2, ISO/IEC 27001:2022, ISO/IEC 27017:2015, ISO/IEC 27018:2019, ISO/IEC 27701:2019, PCI DSS v4.0.1, HIPAA, GDPR, FIPS 140-2, FIPS 140-3, CASA Tier 2, NIST CSF, EU AI Act
tags:
- Company
- Artificial Intelligence
- Agents
- Conversational AI
- Customer Data Platform
- Contact Center
- Machine-Learning
- Large Language Models
- Enterprise Software
- Automation
- Customer Experience
- Knowledge-Management
trust_url: https://trust.uniphore.com/
---
