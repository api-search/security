---
certifications: []
description: ''
kind: trust-center
layout: security
name: Tvscientific Trust Center
name_suffix: Trust Center
overview: Tvscientific maintains a public trust center covering its security and compliance posture.
provider_name: Tvscientific
provider_slug: tvscientific
slug: tvscientific-trust-center
source_filename: tvscientific-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: true\nsource: https://trust.tvscientific.com/\nurl: https://trust.tvscientific.com/\n# The trust center resolves (HTTP 200, page <title>Trust Center</title>, companySlug \"tvscientific\")\n# but is a client-rendered SPA whose framework/certification data loads from an /api/v1/ origin\n# that is not reachable unauthenticated, so named certifications could not be verified.\n# Recorded as a real, published trust center; certifications left empty rather than fabricated.\ncertifications: []\nevidence:\n  - source: https://trust.tvscientific.com/\n    kind: trust-center\n    detail: 'HTTP 200; <title>Trust Center</title>; config.js companySlug \"tvscientific\"'\nnotes: >-\n  Certification list is JavaScript-rendered and not extractable from static HTML;\n  no named certs (SOC 2 / ISO 27001 / PCI DSS / HIPAA / FedRAMP) were verified, so\n  no Compliance pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvscientific/refs/heads/main/security/tvscientific-trust-center.yml
summary_line: trust center published
tags:
- Company
- Advertising
- Connected TV
- CTV
- Streaming
- Performance Marketing
- AdTech
- Measurement
trust_url: https://trust.tvscientific.com/
---
