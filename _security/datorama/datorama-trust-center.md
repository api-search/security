---
certifications:
- SOC 2
- SOC 3
- C5 (ISAE 3000)
- UK Cyber Essentials
- UK Cyber Essentials Plus
- Spain ENS High
- EU Processor Binding Corporate Rules
description: ''
kind: trust-center
layout: security
name: Datorama Trust Center
name_suffix: Trust Center
overview: Datorama maintains a public trust center documenting SOC 2, SOC 3, C5 (ISAE 3000), UK Cyber Essentials, UK Cyber Essentials Plus, Spain ENS High, and EU Processor Binding Corporate Rules compliance.
provider_name: Datorama
provider_slug: datorama
slug: datorama-trust-center
source_filename: datorama-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nurl: https://compliance.salesforce.com/en/services/marketing-cloud-intelligence\ntrust_hub: https://trust.salesforce.com/\nownership_note: >-\n  Salesforce acquired Datorama in August 2018 and runs it as Marketing Cloud Intelligence, so the\n  trust surface is Salesforce's — but it is not generic: the Salesforce compliance site publishes a\n  service page named \"Marketing Cloud - Intelligence\" and four audit documents whose titles name\n  this product explicitly as \"MC Intelligence (fka Datorama)\". Only certifications actually listed\n  under that service page are recorded here.\nprobed: '2026-08-12'\nhttp_status: 200\nservice_scope: Marketing Cloud - Intelligence\ndocuments_total: 55\ndocuments_enumerated: 10\nenumeration_note: >-\n  The service's document table is client-side paginated at 10 rows per page; only page 1 was read,\n  so this is a floor, not a complete list.\ncertifications:\n- SOC 2\n- SOC 3\n- C5 (ISAE\
  \ 3000)\n- UK Cyber Essentials\n- UK Cyber Essentials Plus\n- Spain ENS High\n- EU Processor Binding Corporate Rules\ndatorama_named_documents:\n- {name: 'SOC 2 Report - MC Intelligence (fka Datorama)', updated: '2026-06-16', infrastructure: [AWS, Azure]}\n- {name: 'SOC 3 Report - MC Intelligence (fka Datorama)', updated: '2026-06-16', infrastructure: [AWS, Azure]}\n- {name: 'DR Summary - MC Intelligence (fka Datorama)'}\n- {name: 'Vulnerability/Penetration Report Summary - MC Intelligence (fka Datorama)'}\nother_documents_listed:\n- {name: 'SOC 2 Report - MCE,Intelligence,Advertising,MC Einstein,Personalization,MC Next', updated: '2026-06-16', infrastructure: [AWS, Hyperforce]}\n- {name: 'C5 (ISAE 3000) Report - Marketing Cloud', updated: '2026-06-28', infrastructure: [First party, AWS, Hyperforce]}\n- {name: 'UK Cyber Essentials Certificate', updated: '2026-06-22'}\n- {name: 'UK Cyber Essentials Plus Certificate', updated: '2026-06-22'}\n- {name: 'Spain ENS High - Corporate Services',\
  \ updated: '2026-06-09'}\n- {name: 'Spain ENS High - Marketing Cloud Next', updated: '2026-06-09'}\n- {name: 'Salesforce EU Processor Binding Corporate Rules', updated: '2026-05-06'}\n- {name: 'Salesforce Enterprise Resilience/BCP Summary', updated: '2026-07-23'}\nnot_asserted:\n  note: >-\n    The compliance site's global category taxonomy also names ISO 27001/27017/27018, HIPAA, PCI DSS,\n    FedRAMP, CSA STAR, HITRUST, TISAX, IRAP and others. Those are the catalog's site-wide vocabulary\n    and were NOT shown on the Marketing Cloud - Intelligence document list that was read, so they\n    are deliberately not claimed for this product here.\naccess:\n  gated: false\n  note: >-\n    The service page and document titles are public. Downloading individual audit reports requires a\n    login on compliance.salesforce.com.\nstatus_page: https://status.salesforce.com/products/Datorama\nstatus_page_vanity: https://trust.datorama.com\nevidence:\n- {source: 'https://compliance.salesforce.com/en/services/marketing-cloud-intelligence',\
  \ http_status: 200, keywords: [SOC 2, SOC 3, C5, Cyber Essentials, ENS, Binding Corporate Rules], fetched: '2026-08-12'}\n- {source: 'https://trust.salesforce.com/', http_status: 200, fetched: '2026-08-12'}\n- {source: 'https://trust.datorama.com', http_status: 200, fetched: '2026-08-12', note: '301s to status.salesforce.com/products/Datorama'}\nprobe_result:\n  script: 0-working/probe-security-programs.py\n  run: '2026-08-12'\n  result: 'trust=none'\n  note: >-\n    The mechanical probe found nothing on the datorama.com domain because it redirects to a\n    salesforce.com marketing page. This file is the searched upgrade over that null result.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datorama/refs/heads/main/security/datorama-trust-center.yml
summary_line: SOC 2, SOC 3, C5 (ISAE 3000), UK Cyber Essentials, UK Cyber Essentials Plus, Spain ENS High, EU Processor Binding Corporate Rules
tags:
- Company
- Analytics
- Marketing
- Marketing Intelligence
- Advertising
- Data
- Business Intelligence
- Reporting
- Salesforce
- Marketing Analytics
- Data Harmonization
- Dashboards
- MCP
trust_url: https://compliance.salesforce.com/en/services/marketing-cloud-intelligence
---
