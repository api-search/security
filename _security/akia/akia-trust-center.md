---
certifications:
- SOC 2 Type II
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Akia Trust Center
name_suffix: Trust Center
overview: Akia maintains a public trust center documenting SOC 2 Type II, GDPR, and CCPA compliance.
provider_name: Akia
provider_slug: akia
slug: akia-trust-center
source_filename: akia-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nprobe: true\nsource: https://www.akia.com/security\nurl: https://www.akia.com/security\ncertifications:\n- SOC 2 Type II\n- GDPR\n- CCPA\nposture:\n- claim: SOC 2 Type II\n  detail: Independently audited for security, availability, and confidentiality.\n- claim: Encryption\n  detail: All data encrypted at rest (AES-256) and in transit (TLS 1.3).\n- claim: GDPR Compliant\n  detail: Full compliance with GDPR, CCPA, and other privacy regulations.\n- claim: 99.99% Uptime\n  detail: Enterprise-grade infrastructure with redundancy and failover.\ncontact:\n  security_team: https://www.akia.com/contact\n  security_txt: mailto:security@akia.com\ngaps:\n- 'No dedicated trust portal — trust.akia.com does not resolve. The compliance\n  posture is a marketing section on https://www.akia.com/security with no\n  downloadable report, subprocessor list, or audit-evidence request flow.'\n- 'No status page — status.akia.com does not resolve and no status\
  \ URL is linked\n  from the site, the developer docs, or llms.txt, so the 99.99% uptime claim cannot\n  be checked from outside.'\nevidence:\n- source: https://www.akia.com/security\n  http_status: 200\n  keywords:\n  - soc 2 type ii\n  - gdpr\n  - ccpa\n  - aes-256\n  - tls 1.3\n- source: https://trust.akia.com/\n  http_status: 0\n  note: DNS does not resolve\nx-evidence:\n  fetched: '2026-08-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akia/refs/heads/main/security/akia-trust-center.yml
summary_line: SOC 2 Type II, GDPR, CCPA
tags:
- Company
- Hospitality
- Hotels
- Vacation Rentals
- Guest Experience
- Messaging
- Artificial Intelligence
- Agents
- Property Management
- Check-In
trust_url: https://www.akia.com/security
---
