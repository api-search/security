---
api_specs:
- filename: webscale-networks-webscale-apis-openapi.json
  format: json
  label: Webscale APIs
  slug: webscale-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscale-networks/refs/heads/main/openapi/webscale-networks-webscale-apis-openapi.json
certification_count: 1
certifications:
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Webscale Networks Trust Center
name_suffix: Trust Center
overview: Webscale Networks maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: Webscale Networks
provider_slug: webscale-networks
slug: webscale-networks-trust-center
source_filename: webscale-networks-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://www.webscale.com/security/ (the page that publishes the trust center link)\nname: Webscale Networks trust center\npublished: true\nplatform: Drata\nurl: https://app.drata.com/trust/9cbdd8e2-0c38-11ee-865f-029d78a187d9/workspace/2\nlinked_from: https://www.webscale.com/security/\n\ncertifications:\n- name: SOC 2 Type 2\n  status: certified\n  source: https://www.webscale.com/security/\n  quote: Webscale has earned SOC 2 Type 2 compliance certification.\n\naccess:\n  public_landing: challenged\n  probes:\n  - url: https://app.drata.com/trust/9cbdd8e2-0c38-11ee-865f-029d78a187d9/workspace/2\n    method: GET (curl, browser User-Agent)\n    status: 403\n  - url: https://app.drata.com/trust/9cbdd8e2-0c38-11ee-865f-029d78a187d9/workspace/2\n    method: GET (WebFetch)\n    status: 403\n  finding: >-\n    The trust center is real and published by Webscale — the link is on Webscale's own security page —\n    but the Drata-hosted\
  \ landing page returned 403 to both of our probes with a browser User-Agent.\n    This is Drata's edge bot policy, not a dead link and not a Webscale gating decision, so the\n    certification inventory below could NOT be read from the trust center itself. Every certification\n    recorded here comes from Webscale's own security page instead. Report documents behind a Drata\n    trust center normally require an NDA click-through regardless.\n\ncertifications_read_from_trust_center: false\nsubprocessors_listed: unknown\ndocuments_listed: unknown\n\nnote: >-\n  Recorded as a real trust center with an honest read failure, not as an unverified claim. A later\n  pass with browser automation could enumerate the framework list and document set.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webscale-networks/refs/heads/main/security/webscale-networks-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Ecommerce
- Cloud Hosting
- Content Delivery Network
- Application Delivery
- Web Application Firewall
- Edge Computing
- Managed Hosting
- Infrastructure
- Magento
- Adobe Commerce
- Observability
trust_url: https://app.drata.com/trust/9cbdd8e2-0c38-11ee-865f-029d78a187d9/workspace/2
---
