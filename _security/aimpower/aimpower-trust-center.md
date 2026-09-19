---
certification_count: 0
certifications: []
description: 'Brainsuite operates a public trust centre at trust.brainsuite.ai, hosted by Vanta on its EU tenant (trust-report slug fithz68u9jp7dwx30lhfo, document title "Brainsuite.ai Trust Center"). The page is live and is a real trust report, but its entire body renders client-side: the served HTML is a 5.6KB shell that answers HTTP 200 for every path under the host, and no Vanta JSON endpoint reachable anonymously returns the report content. No certification name could therefore be read, and none is recorded below. Because no certification is readable, no Compliance pointer is emitted for this provider - the trust centre''s existence is a fact; its contents are not something this pass can assert.'
kind: trust-center
layout: security
name: Aimpower Trust Center
name_suffix: Trust Center
overview: Brainsuite.ai maintains a public trust center covering its security and compliance posture.
provider_name: Brainsuite.ai
provider_slug: aimpower
slug: aimpower-trust-center
source_filename: aimpower-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://trust.brainsuite.ai/\ndescription: >-\n  Brainsuite operates a public trust centre at trust.brainsuite.ai, hosted by Vanta on its EU\n  tenant (trust-report slug fithz68u9jp7dwx30lhfo, document title \"Brainsuite.ai Trust\n  Center\"). The page is live and is a real trust report, but its entire body renders\n  client-side: the served HTML is a 5.6KB shell that answers HTTP 200 for every path under\n  the host, and no Vanta JSON endpoint reachable anonymously returns the report content. No\n  certification name could therefore be read, and none is recorded below. Because no\n  certification is readable, no Compliance pointer is emitted for this provider - the trust\n  centre's existence is a fact; its contents are not something this pass can assert.\npresent: true\nurl: https://trust.brainsuite.ai/\nprovider: Vanta (EU tenant)\nhttp_status: 200\nmachine_readable: false\ncertifications: []\ncertifications_readable: false\n\
  subprocessors_published: true\nsubprocessors_url: https://brainsuite.ai/en/data-protection/\nsubprocessors_note: >-\n  The data-protection page names subprocessors in prose - AWS, HubSpot, Google Analytics,\n  LinkedIn, Zendesk, Datadog, Usercentrics, Amazon Cognito and Vimeo - spread across the\n  document rather than in a single table or machine-readable list.\ndata_protection_officer:\n  external: true\n  name: heyData GmbH\n  address: Schuetzenstrasse 5, 10117 Berlin, Germany\n  email: datenschutz@heydata.eu\nposture:\n  gdpr: self-declared\n  hosting: AWS eu-central-1 (Frankfurt am Main, Germany)\n  encryption_at_rest: Amazon SSE-S3, client-specific buckets\n  encryption_in_transit: HTTPS\n  customer_data_used_for_model_training: false\n  customer_data_training_source: >-\n    https://brainsuite.zendesk.com/hc/en-us/articles/22152711650717-Do-you-use-my-data-to-train-AI-models\n  pii: >-\n    The company states it does not work with end-consumer personally identifiable\n    information.\n\
  evidence:\n- url: https://trust.brainsuite.ai/\n  status: 200\n  finding: Live Vanta trust report; contents render client-side only.\n- url: https://brainsuite.ai/.well-known/security.txt\n  status: 404\n  finding: No RFC 9116 security.txt on any company-controlled host.\n- url: https://brainsuite.ai/en/data-protection/\n  status: 200\n  finding: GDPR posture, DPO and subprocessors published; no certification named.\ngaps:\n- No named certification (SOC 2, ISO 27001, TISAX) is readable from any public surface.\n- No security.txt, so no machine-discoverable vulnerability-reporting contact.\n- No bug bounty or coordinated-disclosure page was found on HackerOne, Bugcrowd or Intigriti.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimpower/refs/heads/main/security/aimpower-trust-center.yml
summary_line: trust center published
tags:
- Company
- Advertising
- Marketing
- Artificial Intelligence
- Creative Effectiveness
- Ad Testing
- Market Research
- Consumer Neuroscience
- Media
- Software-as-a-Service
- Germany
trust_url: https://trust.brainsuite.ai/
---
