---
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Hopskipdrive Trust Center
name_suffix: Trust Center
overview: HopSkipDrive maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: HopSkipDrive
provider_slug: hopskipdrive
slug: hopskipdrive-trust-center
source_filename: hopskipdrive-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nurl: https://trust.hopskipdrive.com/\nplatform: Vanta Trust Center\ncertifications:\n- SOC 2 Type II\nframeworks:\n- NIST Cybersecurity Framework\nstatements:\n- text: >-\n    We're proud to have achieved a SOC 2 Type 2 attestation report, demonstrating our\n    commitment to upholding the highest standards of information security. We've\n    implemented a comprehensive suite of administrative, technical, and physical\n    safeguards designed to ensure your data is confidential, maintained with integrity,\n    and available to you when you need it. Our security program aligns with the NIST\n    Cybersecurity Framework.\n  source: https://help.hopskipdrive.com/hc/en-us/articles/44647768425492-HopSkipDrive-Information-Security\nevidence:\n- source: https://trust.hopskipdrive.com/\n  http_status: 200\n  kind: trust-center\n  keywords: [trust center, security, compliance]\n  note: >-\n    Client-rendered Vanta trust report\
  \ (assets.vanta.com/static/index-trust-report.*).\n    The raw HTML carries the title \"HopSkipDrive Trust Center\" and the Vanta signature\n    manifest; the certification list itself renders client-side and was not machine-read,\n    so certifications here are taken from HopSkipDrive's own published statements below.\n- source: https://help.hopskipdrive.com/hc/en-us/articles/44647768425492-HopSkipDrive-Information-Security\n  http_status: 200\n  kind: security-statement\n  keywords: [soc 2 type 2, nist cybersecurity framework]\n- source: https://www.hopskipdrive.com/blog/raising-the-bar-for-data-security-in-student-transportation/\n  http_status: 200\n  kind: announcement\n  keywords: [soc 2 type ii, soc 2 type i, nist cybersecurity framework, encryption in transit and at rest]\n- source: https://www.businesswire.com/news/home/20250402996307/en/HopSkipDrive-Achieves-SOC-2-Type-II-Compliance-Setting-New-Standard-in-Student-Transportation\n  kind: press-release\n  keywords: [soc 2 type\
  \ ii]\ngaps:\n- no_security_txt: /.well-known/security.txt returned 404 on hopskipdrive.com, www.hopskipdrive.com and api.hopskipdrive.com\n- no_public_vulnerability_disclosure_policy: no responsible-disclosure or bug-bounty page found (no HackerOne/Bugcrowd/Intigriti program located)\n- no_published_security_contact: no security@ address published on the public surface\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopskipdrive/refs/heads/main/security/hopskipdrive-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Transportation
- Student Transportation
- Education
- Mobility
- Ridesharing
- School Districts
- Logistics
- Routing
- Government
trust_url: https://trust.hopskipdrive.com/
---
