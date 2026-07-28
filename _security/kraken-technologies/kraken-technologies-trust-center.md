---
certifications:
- ISO/IEC 27001:2022
- SOC 1 Type 2
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Kraken Technologies Trust Center
name_suffix: Trust Center
overview: Kraken Technologies maintains a public trust center documenting ISO/IEC 27001:2022, SOC 1 Type 2, and SOC 2 Type 2 compliance.
provider_name: Kraken Technologies
provider_slug: kraken-technologies
slug: kraken-technologies-trust-center
source_filename: kraken-technologies-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nprobe: true\nurl: https://www.kraken.tech/legal/trust-center\nsource: https://www.kraken.tech/legal/trust-center\nsummary: >-\n  Kraken publishes a substantive Trust Center inside its legal hub (not at trust.kraken.tech, which\n  does not resolve — which is why the automated probe missed it). It names real certifications and\n  attestations, describes the security architecture of the platform, and states that Kraken is a\n  processor whose clients choose deployment region. Reports themselves are available to clients and\n  prospects on request, not for anonymous download.\ncertifications:\n- ISO/IEC 27001:2022\n- SOC 1 Type 2\n- SOC 2 Type 2\ncertification_detail:\n- name: ISO/IEC 27001:2022\n  scope: Information Security Management System (ISMS)\n  verbatim: >-\n    \"Kraken holds ISO/IEC 27001:2022 certification and uses ISO27001 as the basis for our Information\n    Security Management System.\"\n- name: SOC 1 Type 2 / SOC 2 Type\
  \ 2\n  scope: Kraken Customer and Kraken Flex; Security, Availability and Confidentiality criteria\n  cadence: Published twice annually\n  verbatim: >-\n    \"Kraken's Customer and Kraken Flex maintain SOC 1 Type 2 and SOC 2 Type 2 attestations. These\n    reports are published on a twice-annual basis to enable our clients with various reporting\n    schedules to meet their necessary assurance needs.\"\npci_dss:\n  kraken_certified: false\n  model: delegated\n  verbatim: >-\n    \"Credit card processing is not Kraken's mission. This is why we partner with trusted payment\n    providers like Stripe to handle all payment transactions on your behalf... Your card details\n    never touch Kraken's systems, and our payment partners (e.g. Stripe) are certified to the highest\n    industry standards (PCI DSS Level 1).\"\n  note: >-\n    Clients using their own payment provider carry their own PCI compliance. Kraken makes no PCI DSS\n    certification claim for itself.\ndata_protection:\n  gdpr_alignment:\
  \ true\n  verbatim: 'We align with General Data Protection Regulation (GDPR) take this as the standard across the business.'\n  dpo: dpo@kraken.tech\n  privacy_notice: https://www.kraken.tech/legal/privacy-notice\n  cookie_notice: https://www.kraken.tech/legal/cookie-notice\n  dpa: https://www.kraken.tech/legal/dpa\n  subprocessors: https://www.kraken.tech/legal/subprocessors\n  subprocessor_change_notification: true\n  data_residency: >-\n    Clients may deploy Kraken services in any supported region; Kraken will not relocate a client's\n    workspace without prior consent.\n  data_sale: 'Kraken does not sell client data or use it for advertising purposes.'\n  transfer_impact_assessments: documented\nsecurity_architecture:\n  hosting: Amazon Web Services\n  tenancy: >-\n    Kraken Customer Platform and Kraken Field Platform are single-tenant by default, with isolated\n    network virtualisation, dedicated security controls, and optional log feeds into client SIEM\n    tooling.\n  encryption_at_rest:\
  \ AES-256 (databases and other stores, e.g. S3)\n  encryption_in_transit: Mandatory TLS 1.2+; known secure TLS 1.2 cipher suites and TLS 1.3\n  sdlc: >-\n    Secure SDLC integrated into CI/CD with SAST and Software Composition Analysis on every build, and\n    vulnerability analysis before, during and after deployment.\n  patching: Continuous deployment enabling >100 deployments daily, so patches reach client environments quickly.\n  access_control:\n  - Multi-factor authentication across Kraken access points (remote and in office)\n  - Role-based access control with regular privileged access permission audits\n  - Customisable roles and access levels\n  - SAML integration with client identity providers for Kraken Customer Platform\n  security_operations:\n  - Continuous security monitoring\n  - Threat detection with automation and machine learning\n  - Regular security assessments\n  - Incident response procedures and a dedicated security operations team\n  - Disaster recovery capabilities\n\
  \  employee_controls:\n  - Mandatory security and privacy awareness training with annual refreshers\n  - Role-specific security training based on job function and access level\n  - Unique credentials per employee; regular privileged access review\nreport_access:\n  anonymous_download: false\n  channels: [Client Requests, Prospect Requests]\n  note: SOC reports and assurance documentation are provided to clients and prospects on request.\nevidence:\n- source: https://www.kraken.tech/legal/trust-center\n  status: 200\n  date: '2026-07-27'\n  keywords: [trust center, iso/iec 27001:2022, soc 1 type 2, soc 2 type 2, pci dss, gdpr, aes-256, tls 1.2, saml, dpo, subprocessors]\nprobes_that_missed:\n- {host: trust.kraken.tech, dns: NXDOMAIN}\n- {host: security.kraken.tech, dns: NXDOMAIN}\n- {url: 'https://www.kraken.tech/legal/security', status: 200, note: 'legal links only — no certifications; the substance is at /legal/trust-center'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kraken-technologies/refs/heads/main/security/kraken-technologies-trust-center.yml
summary_line: ISO/IEC 27001:2022, SOC 1 Type 2, SOC 2 Type 2
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Demand Response
- DER
- Billing
- Energy Platform
trust_url: https://www.kraken.tech/legal/trust-center
---
