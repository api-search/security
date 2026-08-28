---
certifications:
- SOC 2 Type II
description: Logiwa operates a real, provider-owned Trust Center at trust.logiwa.com, hosted on Vanta. The page is a JavaScript-rendered single-page application, so the control and certification detail it lists is not readable by an anonymous crawler; the certification claim recorded below comes from Logiwa's own marketing site rather than from the Trust Center body.
kind: trust-center
layout: security
name: Logiwa Trust Center
name_suffix: Trust Center
overview: Logiwa maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Logiwa
provider_slug: logiwa
slug: logiwa-trust-center
source_filename: logiwa-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://trust.logiwa.com\nname: Logiwa Trust Center\ndescription: >-\n  Logiwa operates a real, provider-owned Trust Center at trust.logiwa.com, hosted on Vanta. The\n  page is a JavaScript-rendered single-page application, so the control and certification detail\n  it lists is not readable by an anonymous crawler; the certification claim recorded below comes\n  from Logiwa's own marketing site rather than from the Trust Center body.\ntrust_center:\n  url: https://trust.logiwa.com\n  http_status: 200\n  title: Logiwa Trust Center\n  vendor: Vanta\n  vendor_evidence:\n    cname: 664da6b53a3cc20954257c8b.cname.vantatrust.com\n    asset_host: assets.vanta.com\n    slug: 8ilu8co70bc511ucn2w1\n  ownership: >-\n    Provider-controlled subdomain of logiwa.com with a canonical link back to\n    https://trust.logiwa.com and an og:description describing Logiwa IO. This is Logiwa's own\n    trust surface, not a third-party directory listing.\n\
  \  content_readable: false\n  content_note: >-\n    The served HTML is a 7KB SPA shell. Probing /api/trust-center, /api/v1/trust-center and\n    app.vanta.com/api/trust-center/{slug} all returned the same shell (HTTP 200), and\n    api.vanta.com/v1/trust-centers/{slug} returned 401. The control list, subprocessor list and\n    document downloads sit behind Vanta's request/NDA flow. Certifications are therefore NOT\n    enumerated here — only the one Logiwa states publicly.\ncertifications:\n- name: SOC 2 Type II\n  status: claimed-by-provider\n  source: https://www.logiwa.com/solutions/wms-technology-leaders\n  source_http_status: 200\n  evidence: >-\n    Logiwa links a \"SOC 2 Type II Compliance\" resource from its own solutions page. The report\n    itself is not publicly downloadable; access runs through the Trust Center.\n  verified_artifact: false\ncompliance_programs_not_found:\n  note: >-\n    No ISO 27001, PCI DSS, HIPAA, FedRAMP, GDPR-specific or CCPA-specific certification claim\
  \ was\n    found on any anonymously readable Logiwa page. Their absence here means not-found, not\n    not-held — the Trust Center may list more behind its request flow.\n  probed: [iso-27001, pci-dss, hipaa, fedramp, csa-star]\nlegal_documents:\n- name: Privacy Policy\n  url: https://www.logiwa.com/privacy-policy\n  http_status: 200\n- name: Terms of Service\n  url: null\n  http_status: null\n  note: >-\n    NOT PUBLISHED. https://www.logiwa.com/legal (HTTP 200) links only the Privacy Policy.\n    /terms, /terms-of-use, /terms-of-service, /legal/terms, /master-subscription-agreement and\n    /terms-conditions all returned 404, and /terms-and-conditions returned HTTP 200 serving the\n    homepage body — a soft-404, not a terms document. No TermsOfService pointer is claimed.\n- name: DPA / SLA / subprocessor list\n  url: null\n  note: Not linked from the public legal page.\nx-evidence:\n  fetched: '2026-08-25'\n  probes:\n  - url: https://trust.logiwa.com\n    http_status: 200\n  - url:\
  \ https://api.vanta.com/v1/trust-centers/8ilu8co70bc511ucn2w1\n    http_status: 401\n  - url: https://www.logiwa.com/solutions/wms-technology-leaders\n    http_status: 200\n  - url: https://www.logiwa.com/legal\n    http_status: 200\n  - url: https://www.logiwa.com/terms-and-conditions\n    http_status: 200\n    note: Soft-404 — serves homepage content.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logiwa/refs/heads/main/security/logiwa-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Warehouse Management
- Fulfillment
- Logistics
- Supply Chain
- Inventory Management
- Order Management
- Third Party Logistics
- Ecommerce
- Shipping
- Webhooks
- SaaS
trust_url: ''
---
