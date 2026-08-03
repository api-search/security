---
certifications: []
description: ''
kind: trust-center
layout: security
name: Carrum Health Trust Center
name_suffix: Trust Center
overview: Carrum Health maintains a public trust center covering its security and compliance posture.
provider_name: Carrum Health
provider_slug: carrum-health
slug: carrum-health-trust-center
source_filename: carrum-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nprobe: true\nurl: https://trust.carrumhealth.com/\nplatform: Vanta Trust Report\nhttp_status: 200\ncertifications: []\ncertifications_status: not-readable-anonymously\nnotes: >-\n  trust.carrumhealth.com resolves and returns HTTP 200 with a Vanta-hosted trust report\n  shell (data-slugid 2ef014xim0w2hhdngzjeb6, assets served from assets.vanta.com). The\n  certification, control and subprocessor lists are fetched client-side from the Vanta API,\n  which requires authorization (api.vanta.com returns 401 anonymously and its GraphQL\n  endpoint has been retired), so no certification name could be verified. The trust center's\n  existence is confirmed; its contents are deliberately NOT asserted here rather than\n  guessed. Re-run with a JS-capable fetch to enumerate certifications.\n  The automated probe (probe-security-programs.py) did not record this hit because the\n  anonymously served HTML carries fewer than its two-keyword threshold;\
  \ this file was\n  written from a manual verified probe.\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://trust.carrumhealth.com/\n  http_status: 200\n  content_type: text/html\n  tls: TLSv1.3\n  hsts: max-age=31536000; includeSubDomains\n  markers:\n  - assets.vanta.com/static/index-trust-report\n  - data-slugid=\"2ef014xim0w2hhdngzjeb6\"\n  - '<meta name=\"keywords\" content=\"Trust, Security, Compliance, Automation\">'\nvulnerability_disclosure:\n  present: false\n  probed:\n  - {url: 'https://carrumhealth.com/.well-known/security.txt', status: 404}\n  - {url: 'https://carrumhealth.com/security.txt', status: 404}\n  - {url: 'https://carrumhealth.com/security', status: 404}\n  - {url: 'https://carrumhealth.com/responsible-disclosure', status: 404}\n  - {url: 'https://carrumhealth.com/vulnerability-disclosure', status: 404}\n  - {url: 'https://hackerone.com/carrumhealth', status: 404}\n  - {url: 'https://bugcrowd.com/carrumhealth', status: 404}\n  note: >-\n    No security.txt, no\
  \ disclosure page and no bug-bounty program was found, so no\n    vulnerability-disclosure artifact and no `Security` pointer was written.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carrum-health/refs/heads/main/security/carrum-health-trust-center.yml
summary_line: trust center published
tags:
- Company
- Healthcare
- Health Benefits
- Centers of Excellence
- Value-Based Care
- Bundled Payments
- Employee Benefits
- Surgery
- Care Navigation
- Digital Health
trust_url: https://trust.carrumhealth.com/
---
