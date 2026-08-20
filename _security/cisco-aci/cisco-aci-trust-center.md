---
certifications:
- Common Criteria EAL2+ (ALC_FLR.2)
- Common Criteria EAL2
- FIPS 140 (certificate 4747)
- FIPS 140
description: ''
kind: trust-center
layout: security
name: Cisco Aci Trust Center
name_suffix: Trust Center
overview: Cisco ACI maintains a public trust center documenting Common Criteria EAL2+ (ALC_FLR.2), Common Criteria EAL2, FIPS 140 (certificate 4747), and FIPS 140 compliance.
provider_name: Cisco ACI
provider_slug: cisco-aci
slug: cisco-aci-trust-center
source_filename: cisco-aci-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://www.cisco.com/c/en/us/about/trust-center.html\nnote: >-\n  The automated trust-center probe (probe-security-programs.py) returned no hit for this slug, because\n  Cisco's trust surface is not at trust.cisco.com or /trust — it is split across the Trust Center, a separate\n  Trust Portal on its own hostname, and the Global Government Certifications pages where the\n  product-specific certifications actually live. All four were fetched and verified by hand on 2026-08-19.\n  The certifications recorded below name Cisco ACI / APIC explicitly; Cisco-wide programs that do not name\n  this product are noted as such rather than credited to it.\ntrust_center:\n  url: https://www.cisco.com/c/en/us/about/trust-center.html\n  status: 200\ntrust_portal:\n  url: https://trustportal.cisco.com/\n  status: 200\n  detail: >-\n    Self-service access to Cisco's security, data-privacy and compliance documents. Document retrieval is\n  \
  \  behind the portal UI, not a machine-readable feed.\ncompliance_page:\n  url: https://www.cisco.com/c/en/us/about/trust-center/compliance.html\n  status: 200\n  detail: >-\n    Describes the Cisco Cloud Controls Framework (CCF), a \"build-once-use-many\" control set Cisco uses to\n    certify SaaS solutions, and links to the Trust Portal. The served HTML is a thin shell — the certified\n    solution list renders client-side, so it is not readable by a machine.\ncertifications:\n- name: Common Criteria EAL2+ (ALC_FLR.2)\n  scope: Cisco N9000 Switch Series with ACI mode, APIC 6.1(2g) and NX-OS software-ACI 16.1(2g)\n  certified: '2025-05-16'\n  expires: '2030-05-16'\n  product_named: true\n  source: https://www.cisco.com/c/en/us/solutions/industries/government/global-government-certifications/common-criteria.html\n- name: Common Criteria EAL2\n  scope: Cisco N9000 Switch Series with ACI mode, APIC and Nexus 2000 Fabric Extenders (NSCIB-21-163806)\n  certified: '2021-02-02'\n  expires:\
  \ '2026-02-02'\n  product_named: true\n  source: https://www.cisco.com/c/en/us/solutions/industries/government/global-government-certifications/common-criteria.html\n- name: FIPS 140 (certificate 4747)\n  scope: APIC/ACI Controller running v6.1\n  certified: '2025-06-16'\n  product_named: true\n  source: https://www.cisco.com/c/en/us/solutions/industries/government/global-government-certifications/fips-140.html\n- name: FIPS 140\n  scope: N9000 APIC/ACI Controller running v6.0\n  certified: '2022-09-26'\n  product_named: true\n  source: https://www.cisco.com/c/en/us/solutions/industries/government/global-government-certifications/fips-140.html\nprograms:\n- name: Cisco Cloud Controls Framework (CCF)\n  product_named: false\n  detail: Cisco-wide control framework for SaaS certification. Not ACI-specific.\n  url: https://www.cisco.com/c/en/us/about/trust-center/compliance.html\n- name: Cisco PSIRT security vulnerability policy\n  product_named: false\n  url: https://sec.cloudapps.cisco.com/security/center/resources/security_vulnerability_policy.html\n\
  - name: CSAF advisory publication\n  product_named: false\n  detail: >-\n    Cisco publishes machine-readable security advisories under the Common Security Advisory Framework,\n    advertised from security.txt.\n  url: https://www.cisco.com/.well-known/csaf/provider-metadata.json\nmachine_readable:\n  certifications_feed: false\n  detail: >-\n    Every certification above was read out of an HTML table on a marketing page. There is no JSON/CSV feed\n    of Cisco certifications, and the Trust Portal does not expose an anonymous API — an agent cannot verify\n    a Cisco compliance claim without a human in the loop.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-aci/refs/heads/main/security/cisco-aci-trust-center.yml
summary_line: Common Criteria EAL2+ (ALC_FLR.2), Common Criteria EAL2, FIPS 140 (certificate 4747), FIPS 140
tags:
- SDN
- Data-Center
- Networking
- Fabric
- Automation
- Enterprise
- Network Automation
- Infrastructure
- Controller
- REST API
trust_url: ''
---
