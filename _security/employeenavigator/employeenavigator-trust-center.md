---
certifications:
- SOC 2 Type II
- HITRUST
- HIPAA
- GDPR
- CCPA
- 23 NYCRR 500 (NYDFS)
- NIST
description: ''
kind: trust-center
layout: security
name: Employeenavigator Trust Center
name_suffix: Trust Center
overview: Employee Navigator maintains a public trust center documenting SOC 2 Type II, HITRUST, HIPAA, GDPR, CCPA, 23 NYCRR 500 (NYDFS), and NIST compliance.
provider_name: Employee Navigator
provider_slug: employeenavigator
slug: employeenavigator-trust-center
source_filename: employeenavigator-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nprobe: true\nsource: https://www.employeenavigator.com/security/\nurl: https://www.employeenavigator.com/security/\nsummary: >-\n  Employee Navigator publishes a single public security and compliance page\n  rather than a hosted trust portal. It names the audit and certification program,\n  the cloud platform and its encryption posture, and the operational controls,\n  but it does not offer document download, subgroup reporting, or a\n  vulnerability-disclosure channel.\ncertifications:\n- SOC 2 Type II\n- HITRUST\n- HIPAA\n- GDPR\n- CCPA\n- 23 NYCRR 500 (NYDFS)\n- NIST\naudit_cadence: annual\ninfrastructure:\n  cloud: Microsoft Azure\n  managed_hosting: Logicworks (managed Azure external public cloud datacenter hosting)\n  encryption_at_rest: Azure Storage Service Encryption, AES 256-bit, Microsoft-managed keys\n  encryption_in_transit: TLS 1.2+ on all connections; HTTP auto-redirects to HTTPS\ncontrols:\n- Formalized hiring practice\
  \ with third-party background checks on all employees\n- Least-privilege access management with mandatory two-factor authentication\n- Physical datacenter access expressly prohibited to staff\n- Implicit deny-all network access control with perimeter firewall and VPN appliances\n- Customer environment isolation (licensees may access only their assigned environment)\n- Centralized SIEM log correlation, analysis and alerting with 24x7 security engineer response\n- Disk-to-disk on-site backup, daily cross-datacenter replication, high-availability database cluster\ndata_handling:\n- All licensee data classified equally as sensitive; no data classification performed on behalf of licensees\n- Employee Navigator staff do not access licensee data outside explicit customer request\n- No customer data shared with external third parties unless customer-requested or legally required\n- 'Partner transport protocols: API, SSL file upload, and SFTP/FTP with PGP, with optional approved static IPs'\ngaps:\n\
  - No /.well-known/security.txt (RFC 9116)\n- No published vulnerability-disclosure or responsible-disclosure policy\n- No bug bounty program found on HackerOne, Bugcrowd or Intigriti\n- No named security contact address; the only published address is sales@employeenavigator.com\n- No downloadable attestation reports or hosted trust portal\n- No public status page (employeenavigator.statuspage.io returns page-deleted)\nevidence:\n- source: https://www.employeenavigator.com/security/\n  http_status: 200\n  keywords:\n  - soc 2 type ii\n  - hitrust\n  - nist\n  - gdpr\n  - 23 nycrr 500\n  - ccpa\n  - hipaa\n  - compliance certifications and attestations\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://www.employeenavigator.com/security/\n  http_status: 200\n  content_type: text/html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/employeenavigator/refs/heads/main/security/employeenavigator-trust-center.yml
summary_line: SOC 2 Type II, HITRUST, HIPAA, GDPR, CCPA, 23 NYCRR 500 (NYDFS), NIST
tags:
- Company
- Benefits Administration
- Human Resources
- Insurance
- Employee Benefits
- Payroll
- Health Insurance
- HRIS
- Open Enrollment
- ACA Compliance
- Identity
- OpenID Connect
trust_url: https://www.employeenavigator.com/security/
---
