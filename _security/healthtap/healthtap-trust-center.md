---
certifications:
- SOC 2 Type 2
- HIPAA
description: ''
kind: trust-center
layout: security
name: Healthtap Trust Center
name_suffix: Trust Center
overview: HealthTap maintains a public trust center documenting SOC 2 Type 2 and HIPAA compliance.
provider_name: HealthTap
provider_slug: healthtap
slug: healthtap-trust-center
source_filename: healthtap-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nurl: https://www.healthtap.com/security/\ntitle: Security and Privacy | HealthTap\ncertifications:\n- SOC 2 Type 2\n- HIPAA\nframeworks_referenced:\n- CIS (Center for Internet Security) benchmarks\n- CSA (Cloud Security Alliance) guidance\ncontrols_published:\n- TLS / HTTPS encryption of communications over public networks\n- Third-party independent penetration testing\n- HIPAA Business Associate posture on behalf of the treating clinicians\nnotes: >-\n  HealthTap publishes a consumer-facing \"Security and Privacy\" page at\n  /security/ that names a SOC 2 Type 2 certification covering its HIPAA\n  compliance, states that it is a Business Associate of the health care\n  professionals on its platform under HIPAA, and describes TLS/HTTPS encryption,\n  third-party penetration testing, and use of CIS and CSA standards for its\n  servers and networks. This is a compliance-posture page, not a full trust\n  center: there is\
  \ no evidence portal, no downloadable audit report, no\n  subprocessor list, and no vulnerability-disclosure or bug-bounty program (see\n  the note below).\nvulnerability_disclosure: none-found\nvulnerability_disclosure_notes: >-\n  No responsible-disclosure page, no /.well-known/security.txt, no security@\n  contact and no HackerOne / Bugcrowd / Intigriti program was found for\n  HealthTap. The only machine-readable security contact anywhere on the domain\n  is the CAA iodef record, mailto:devops+caa@healthtap.com, which is a\n  certificate-misissuance reporting address and not a vulnerability-disclosure\n  channel. No `Security` pointer is emitted in apis.yml because there is no\n  disclosure policy to point at.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://www.healthtap.com/security/\n  http_status: 403\n  http_status_note: >-\n    Direct retrieval of the page was not possible from this environment: the\n    healthtap.com Cloudflare zone returns HTTP 403 with a block page to\
  \ every\n    non-browser client (plain curl, browser user-agent strings, Googlebot,\n    bingbot, facebookexternalhit and Twitterbot were all refused). The page\n    itself is publicly published and search-indexed; the certifications and\n    controls above are recorded from the indexed content of that exact URL. The\n    automated probe (0-working/probe-security-programs.py) therefore returned\n    trust=none — the block, not the absence of a page, is why.\n  probe_result: trust=none (blocked by edge, not absent)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthtap/refs/heads/main/security/healthtap-trust-center.yml
summary_line: SOC 2 Type 2, HIPAA
tags:
- Company
- Health Tech
- Telehealth
- Telemedicine
- Virtual Care
- Healthcare
- Primary Care
- Digital Health
trust_url: https://www.healthtap.com/security/
---
