---
certifications: []
description: ''
kind: trust-center
layout: security
name: Sundaysky Trust Center
name_suffix: Trust Center
overview: SundaySky maintains a public trust center covering its security and compliance posture.
provider_name: SundaySky
provider_slug: sundaysky
slug: sundaysky-trust-center
source_filename: sundaysky-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nprobe: true\nurl: https://trust.sundaysky.com/\nhttp_status: 200\nfetched: '2026-08-13'\n\nplatform: Scytale\nplatform_evidence: >-\n  The trust center is a client-rendered React application whose bundle declares\n  API_URL \"https://api.scytale.ai\", TRUST_CENTER_DOMAIN \"trustcenter.scytale.ai\",\n  version 1.0.69, and carries the string \"trust-center.powered-by-scytale\".\n  Read from https://trust.sundaysky.com/main.8f323eb1d028c9a65ab0.js on\n  2026-08-13.\n\nsections_advertised:\n- Compliance\n- Controls\n- Policies\n- Reports and Documents\n- FAQ\n\naccess_model: request-access\naccess_note: >-\n  The trust center presents a request-access dialog collecting full name, email\n  and company name. The bundle distinguishes public from restricted files\n  (\"trust-center.file.public\" / \"trust-center.file.restricted\"), so some\n  documents may be public to a browser session — but no certification name,\n  control, or document title\
  \ is present in any anonymously reachable response.\n\ncertifications: []\ncertifications_note: >-\n  NONE VERIFIED. The section labels above are UI strings from the application\n  bundle, not SundaySky's actual compliance content. The content itself is\n  fetched at runtime from api.scytale.ai and was not retrievable anonymously:\n  the tenant-resolution call could not be reproduced without the application's\n  own request context. Recording a certification here without seeing it served\n  would be fabrication, so the list is deliberately empty.\n  CONSEQUENCE: no `Compliance` pointer is emitted in apis.yml. The\n  `compliance_published` check should score zero for this provider until a named\n  certification is verified. A `TrustCenter` pointer IS emitted, because the\n  trust center's existence is directly verified.\n\ncorroborating_evidence:\n  help_center_certification_sweep:\n    corpus: 233 help center articles\n    fetched: '2026-08-13'\n    pattern: SOC 2, SOC 1, ISO 27001, PCI\
  \ DSS, HIPAA, FedRAMP, GDPR, CCPA, CSA STAR, FIPS 140\n    named_certifications_found: 0\n    note: >-\n      The only matches across the entire corpus were WCAG (accessibility) and a\n      single incidental HIPAA mention inside the Third Party Terms article. No\n      SOC 2 or ISO 27001 claim appears anywhere in SundaySky's public\n      documentation, which is consistent with the certification detail living\n      behind the trust center's access gate.\n\nevidence:\n- source: https://trust.sundaysky.com/\n  http_status: 200\n  kind: trust-center\n  finding: >-\n    Live trust center at the conventional trust.<domain> subdomain, titled\n    \"Trust Center\", serving a 545-byte shell plus three JS bundles.\n- source: https://trust.sundaysky.com/main.8f323eb1d028c9a65ab0.js\n  http_status: 200\n  kind: bundle\n  finding: Scytale platform identification and section taxonomy.\n- source: https://sundaysky.com/security/\n  http_status: 200\n  kind: false-positive\n  finding: >-\n    NOT a\
  \ security page. This path 302s to\n    https://sundaysky.com/wp-content/uploads/2024/08/Security.png and returns a\n    101KB PNG image with content-type image/png. A status-code-only probe would\n    wrongly record a security page here.\n\nrelated:\n  domain_security: security/sundaysky-domain-security.yml\n  conformance: conformance/sundaysky-conformance.yml\n  vulnerability_disclosure:\n    published: false\n    note: >-\n      No vulnerability disclosure program found. probe-security-programs.py\n      returned vdp=none on 2026-08-13. No security.txt is served on any host, no\n      security@ address is published in the help center, and no HackerOne,\n      Bugcrowd, or Intigriti program was found. No Security or\n      VulnerabilityDisclosure pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sundaysky/refs/heads/main/security/sundaysky-trust-center.yml
summary_line: trust center published
tags:
- Company
- Video
- Personalization
- Video Personalization
- Marketing
- Customer Experience
- Artificial Intelligence
- Enterprise
- Video Generation
- Media
- Analytics
- Martech
trust_url: https://trust.sundaysky.com/
---
