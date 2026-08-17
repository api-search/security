---
api_specs:
- filename: freshpaint-events-api-openapi.yml
  format: yaml
  label: Freshpaint Events API
  slug: freshpaint-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/openapi/freshpaint-events-api-openapi.yml
certifications:
- SOC 2 Type 2
- HIPAA
description: Freshpaint runs a real, self-service trust center at trust.freshpaint.io with named certifications, downloadable audit artifacts, and an enumerated control set. This is the strongest single piece of Freshpaint's public posture and the reason a Compliance pointer is wired — it is a published compliance program, not an inferred one.
kind: trust-center
layout: security
name: Freshpaint Trust Center
name_suffix: Trust Center
overview: Freshpaint maintains a public trust center documenting SOC 2 Type 2 and HIPAA compliance.
provider_name: Freshpaint
provider_slug: freshpaint
slug: freshpaint-trust-center
source_filename: freshpaint-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://trust.freshpaint.io/\nurl: https://trust.freshpaint.io/\nhttp_status: 200\nfetched: '2026-08-13'\ndescription: >-\n  Freshpaint runs a real, self-service trust center at trust.freshpaint.io with\n  named certifications, downloadable audit artifacts, and an enumerated control\n  set. This is the strongest single piece of Freshpaint's public posture and\n  the reason a Compliance pointer is wired — it is a published compliance\n  program, not an inferred one.\ncertifications:\n- SOC 2 Type 2\n- HIPAA\nin_progress:\n- name: HITRUST r2\n  note: >-\n    The trust center states Freshpaint \"is actively working toward HITRUST r2\n    certification\". Recorded as in-progress, not as a held certification.\ndocuments:\n- name: SOC 2 Report\n- name: Pentest Report\n- name: Security Prospectus\ncontrols:\n- Encryption at rest\n- Encryption in transit\n- Access log management\n- Automated account management\n- Virtual\
  \ private cloud\n- Traffic filtering\n- Web application firewall\n- Software development lifecycle\n- Code analysis\n- Endpoint detection and response\n- Mobile device management\n- Incident response\n- Penetration testing\n- Employee training\nprograms:\n- name: Vulnerability Management Program\n  description: >-\n    Freshpaint maintains a vulnerability management program to identify,\n    assess, remediate, verify, and report technical vulnerabilities.\n  note: >-\n    This is an INTERNAL vulnerability management program. It is not a public\n    vulnerability disclosure program — see gaps below.\n- name: Security Awareness Training Program\n- name: Endpoint Security and Device Management Program\nsubprocessors:\n  section_present: true\n  list_captured: false\n  note: A Subprocessors section is referenced on the trust center but no list was returned in the fetched content.\ngaps:\n- >-\n  No vulnerability disclosure or bug bounty program is named anywhere on the\n  trust center, and\
  \ no security contact email is published. /.well-known/\n  security.txt returns 404 on freshpaint.io, www.freshpaint.io and\n  trust.freshpaint.io, and /security, /responsible-disclosure,\n  /security/responsible-disclosure and /vulnerability-disclosure all return 404\n  on www.freshpaint.io. A researcher who finds a bug in a HIPAA-scoped platform\n  has no published route to report it. No Security or VulnerabilityDisclosure\n  pointer is wired, because there is nothing to point at.\nevidence:\n- source: https://trust.freshpaint.io/\n  http_status: 200\n  fetched: '2026-08-13'\n  keywords: [soc 2 type 2, hipaa, hitrust r2, trust center, pentest report, vulnerability management]\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/security/freshpaint-trust-center.yml
summary_line: SOC 2 Type 2, HIPAA
tags:
- Customer Data Platform
- Event Tracking
- Healthcare
- HIPAA
- Privacy
- Analytics
trust_url: https://trust.freshpaint.io/
---
