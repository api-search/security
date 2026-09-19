---
certification_count: 2
certifications:
- named_publicly
- note
description: ''
kind: trust-center
layout: security
name: Hologic Trust Center
name_suffix: Trust Center
overview: Hologic maintains a public trust center documenting named_publicly and note compliance.
provider_name: Hologic
provider_slug: hologic
slug: hologic-trust-center
source_filename: hologic-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: https://www.hologic.com/support/usa/breast-skeletal-products-cybersecurity\nnote: >-\n  Hologic publishes no trust center in the SaaS sense — there is no trust.hologic.com, no\n  SOC 2 / ISO 27001 report request portal, and no compliance-document download gateway. Probed\n  https://www.hologic.com/trust (404), /security (404), /cybersecurity (404) and\n  /product-security (404); 0-working/probe-security-programs.py likewise returned trust=none.\n  What stands in its place is a product-security hub scoped to the Breast & Skeletal Health\n  division, which is where a medical device buyer's security review actually lands.\ntrust_center:\n  exists: false\n  equivalent:\n    name: Breast & Skeletal Products Cybersecurity\n    url: https://www.hologic.com/support/usa/breast-skeletal-products-cybersecurity\n    http_status: 200\n    scope: Breast and Skeletal Health division products only — not company-wide.\n    contents:\n     \
  \ - Coordinated Vulnerability Disclosure Policy\n      - MDS2 security disclosure forms, per product (36 linked)\n      - Cybersecurity reports and best-practice guides, per product\n      - Validated Microsoft monthly critical patch releases\n      - Antivirus installation and configuration guides\n      - Dated security advisories for third-party CVEs affecting Hologic products\ncertifications:\n  named_publicly: []\n  note: >-\n    No SOC 2, ISO 27001, ISO 13485, PCI DSS, HIPAA attestation or FedRAMP authorization is\n    named on any public Hologic page reached by this pass. Regulatory posture is expressed\n    instead as FDA 510(k) clearance and CE marking per device, and as per-product MDS2 forms.\n    Absence here is a publication finding, not a claim that Hologic holds no certifications.\nprobes:\n  - url: https://www.hologic.com/trust\n    status: 404\n  - url: https://www.hologic.com/security\n    status: 404\n  - url: https://www.hologic.com/cybersecurity\n    status: 404\n\
  \  - url: https://www.hologic.com/product-security\n    status: 404\n  - url: https://www.hologic.com/support/usa/breast-skeletal-products-cybersecurity\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hologic/refs/heads/main/security/hologic-trust-center.yml
summary_line: named_publicly, note
tags:
- Fortune 1000
- Healthcare
- Medical Devices
- Medical Imaging
- Diagnostics
- Women's Health
- DICOM
- Life Sciences
trust_url: ''
---
