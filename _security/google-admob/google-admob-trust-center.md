---
api_specs:
- filename: google-admob-accounts-api-openapi.yml
  format: yaml
  label: Google AdMob Accounts API
  slug: google-admob-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-admob/openapi/google-admob-accounts-api-openapi.yml
certification_count: 8
certifications:
- ISO/IEC 27001
- ISO/IEC 27017
- ISO/IEC 27018
- ISO/IEC 27701
- SOC 2 / SOC 3
- SOC 1 Type 2
- FedRAMP
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Google AdMob Trust Center
name_suffix: Trust Center
overview: Google AdMob maintains a public trust center documenting ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, ISO/IEC 27701, SOC 2 / SOC 3, SOC 1 Type 2, FedRAMP, and PCI DSS compliance.
provider_name: Google AdMob
provider_slug: google-admob
slug: google-admob-trust-center
source_filename: google-admob-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://business.safety.google/compliance/\nalso:\n- https://privacy.google.com/businesses/compliance/\n- https://safety.google/security/\nnotes: 'AdMob has no trust center of its own — trust.admob.google.com and security.admob.google.com do not exist, and the automated probe over\n  admob.google.com and developers.google.com found no trust/compliance page (probe-security-programs.py, 2026-08-13, trust=none). What Google\n  DOES publish is a business-wide compliance page at business.safety.google/compliance/, fetched 2026-08-13, which names certifications and states\n  their scope product-by-product. SCOPE CAVEAT, recorded deliberately: AdMob is NOT named on that page. Google Ads appears in the ISO 27001 scope\n  statement, and AdWords and AdSense appear in the SOC 1 Type 2 scope; AdMob appears in neither. Do not read this artifact as a certification\n  claim for admob.googleapis.com — read it as \"Google publishes\
  \ a compliance program covering its advertising business, and AdMob is not enumerated\n  in it.\"'\ncertifications:\n- ISO/IEC 27001\n- ISO/IEC 27017\n- ISO/IEC 27018\n- ISO/IEC 27701\n- SOC 2 / SOC 3\n- SOC 1 Type 2\n- FedRAMP\n- PCI DSS\nnot_listed:\n- HIPAA\n- CSA STAR\ndata_protection_terms:\n  ads_controller_terms: https://business.safety.google/adscontrollerterms/\n  privacy_policy: https://policies.google.com/privacy\nevidence:\n- source: https://business.safety.google/compliance/\n  status: 200\n  keywords:\n  - iso 27001\n  - soc 2\n  - soc 1 type 2\n  - fedramp\n  - pci dss\n- source: https://privacy.google.com/businesses/compliance/\n  status: 200\n- source: https://trust.admob.google.com/\n  status: dns-nxdomain\n  note: 'Probed 2026-08-13: no A record, connection failed (curl 000). No AdMob-specific trust center exists.'\n- source: https://security.admob.google.com/\n  status: dns-nxdomain\n  note: 'Probed 2026-08-13: no A record, connection failed (curl 000).'\ncertifications_detail:\n\
  - name: ISO/IEC 27001\n  scope_stated: Google Cloud Platform, Google Workspace, Google Ads\n  admob_named: false\n- name: ISO/IEC 27017\n  scope_stated: Google Cloud Platform, Google Workspace\n  admob_named: false\n- name: ISO/IEC 27018\n  scope_stated: Google Cloud Platform, Google Workspace\n  admob_named: false\n- name: ISO/IEC 27701\n  scope_stated: Google Cloud Platform, Google Workspace\n  admob_named: false\n- name: SOC 2 / SOC 3\n  scope_stated: Google Cloud Platform, Google Workspace\n  admob_named: false\n- name: SOC 1 Type 2\n  scope_stated: AdWords, AdSense, Google Cloud Platform, Google Workspace, DoubleClick Campaign Manager, DoubleClick for Publishers, DoubleClick\n    Ad Exchange\n  admob_named: false\n- name: FedRAMP\n  scope_stated: Google Workspace, Google Cloud Platform\n  admob_named: false\n- name: PCI DSS\n  scope_stated: Google Cloud Platform, Android Pay\n  admob_named: false\nsource: https://business.safety.google/compliance/\n"
source_yaml_url: https://artifacts.apis.io/google-admob/security/google-admob-trust-center.yml
summary_line: ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, ISO/IEC 27701, SOC 2 / SOC 3, SOC 1 Type 2, FedRAMP, PCI DSS
tags:
- Ad Mediation
- AdMob
- Advertising
- App Monetization
- Mobile Advertising
- Mobile App
- Reports
- Reporting
trust_url: https://business.safety.google/compliance/
---
