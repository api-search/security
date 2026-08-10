---
certifications:
- SOC 2
description: ''
kind: trust-center
layout: security
name: Pebblepost Trust Center
name_suffix: Trust Center
overview: PebblePost maintains a public trust center documenting SOC 2 compliance.
provider_name: PebblePost
provider_slug: pebblepost
slug: pebblepost-trust-center
source_filename: pebblepost-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nsource: https://trust.pebblepost.com/\nurl: https://trust.pebblepost.com/\nplatform: Vanta Trust Center\ntitle: PebblePost Trust Center\n# Certifications could NOT be enumerated anonymously. The trust report is a Vanta\n# single-page app; its content is served from a signed GraphQL endpoint that rejects\n# unsigned requests (\"Missing `signature` or `signedAt`\", HTTP 400), so no certification\n# list is machine-readable from the public page. The one certification claim PebblePost\n# publishes in plain HTML is the SOC 2 statement in its privacy policy, recorded below.\ncertifications:\n- SOC 2\ncertification_evidence:\n- certification: SOC 2\n  source: https://www.pebblepost.com/privacy-policy/\n  quote: 'PebblePost maintains and has placed controls within its Services that upholds\n    commitments and system requirements for SOC 2 compliance.'\n  note: A compliance claim in the privacy policy, not an audit report or a\
  \ certificate\n    number. PebblePost links to the AICPA SOC suite overview page rather than to its\n    own report.\n  reference: https://www.aicpa-cima.com/resources/landing/system-and-organization-controls-soc-suite-of-services\nevidence:\n- source: https://trust.pebblepost.com/\n  http_status: 200\n  content_type: text/html\n  observed: 'Vanta-hosted trust center; page <title> is \"PebblePost Trust Center\";\n    assets served from assets.vanta.com; canonical https://trust.pebblepost.com'\n- source: https://trust.pebblepost.com/graphql\n  http_status: 400\n  observed: 'GraphQL rejects unsigned requests: {\"errors\":[{\"message\":\"Missing `signature`\n    or `signedAt`\"}]} — report contents are not anonymously readable'\n- source: https://www.pebblepost.com/privacy-policy/\n  http_status: 200\n  observed: SOC 2 compliance statement in the Security section\nx-gap:\n  - The trust center exists but publishes nothing a machine can read anonymously.\n    Named certifications, audit dates\
  \ and subprocessors are all behind Vanta's signed\n    report. Publishing the certification list in the page's static HTML (or an\n    accompanying /.well-known/security.txt) would make the posture verifiable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pebblepost/refs/heads/main/security/pebblepost-trust-center.yml
summary_line: SOC 2
tags:
- Company
- Marketing
- Advertising
- Direct Mail
- Connected TV
- Retail
- Commerce
- Identity
- Analytics
trust_url: https://trust.pebblepost.com/
---
