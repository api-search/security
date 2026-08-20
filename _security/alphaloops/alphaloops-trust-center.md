---
api_specs:
- filename: alphaloops-fmcsa-carrier-data-api-carriers-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Carriers API
  slug: alphaloops-fmcsa-carrier-data-api-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-fmcsa-carrier-data-api-carriers-api-openapi.yml
- filename: alphaloops-fmcsa-carrier-data-api-contacts-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Contacts API
  slug: alphaloops-fmcsa-carrier-data-api-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-fmcsa-carrier-data-api-contacts-api-openapi.yml
- filename: alphaloops-fmcsa-carrier-data-api-inspections-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Inspections API
  slug: alphaloops-fmcsa-carrier-data-api-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-fmcsa-carrier-data-api-inspections-api-openapi.yml
- filename: alphaloops-fmcsa-carrier-data-api-vins-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Vins API
  slug: alphaloops-fmcsa-carrier-data-api-vins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-fmcsa-carrier-data-api-vins-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
- NIST Cybersecurity Framework
- COBIT
description: AlphaLoops publishes a security page at https://runalphaloops.com/security and operates a Vanta-hosted Trust Center at https://trust.runalphaloops.com/ (linked from the site footer). The Trust Center returned HTTP 200 but is fully client-rendered — no certification names, control list, or document index are present in the served HTML, and the Vanta trust-page API paths probed anonymously return the SPA shell rather than JSON. The certifications below are therefore read from the PUBLIC SECURITY PAGE, not from the Trust Center itself.
kind: trust-center
layout: security
name: Alphaloops Trust Center
name_suffix: Trust Center
overview: AlphaLoops FMCSA Carrier Data API maintains a public trust center documenting SOC 2 Type II, ISO 27001, NIST Cybersecurity Framework, and COBIT compliance.
provider_name: AlphaLoops FMCSA Carrier Data API
provider_slug: alphaloops
slug: alphaloops-trust-center
source_filename: alphaloops-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nprobe: true\nsource: https://runalphaloops.com/security\nurl: https://trust.runalphaloops.com/\ndescription: >-\n  AlphaLoops publishes a security page at https://runalphaloops.com/security and operates a\n  Vanta-hosted Trust Center at https://trust.runalphaloops.com/ (linked from the site footer).\n  The Trust Center returned HTTP 200 but is fully client-rendered — no certification names,\n  control list, or document index are present in the served HTML, and the Vanta trust-page API\n  paths probed anonymously return the SPA shell rather than JSON. The certifications below are\n  therefore read from the PUBLIC SECURITY PAGE, not from the Trust Center itself.\n\n# IMPORTANT — these are the claims as WORDED by the provider. AlphaLoops describes itself as\n# \"aligned with\" ISO 27001 and built on \"SOC 2 certified infrastructure\". That is a posture\n# statement about controls and about its cloud vendors; it is NOT an assertion that\
  \ AlphaLoops\n# itself holds a SOC 2 or ISO 27001 certificate, and no audit report, certificate number, or\n# auditor is named on any public page. Recorded verbatim so the distinction is not lost.\ncertifications:\n  - name: SOC 2 Type II\n    claim: infrastructure\n    status: claimed-alignment\n    verbatim: 'SOC 2 Type II infrastructure'\n    certificate_published: false\n    note: >-\n      Stated as the compliance posture of the underlying infrastructure. No SOC 2 report,\n      certificate, or auditor is named on a public page, and the Trust Center that would\n      normally host the report is not machine-readable.\n  - name: ISO 27001\n    claim: aligned\n    status: claimed-alignment\n    verbatim: 'ISO 27001 aligned controls'\n    certificate_published: false\n    note: Described as \"aligned with\" / \"aligned controls\" — not stated as a held certification.\n  - name: NIST Cybersecurity Framework\n    claim: aligned\n    status: claimed-alignment\n    verbatim: 'NIST Cybersecurity\
  \ Framework'\n    certificate_published: false\n  - name: COBIT\n    claim: aligned\n    status: claimed-alignment\n    verbatim: 'COBIT governance domains'\n    certificate_published: false\n\n# Privacy regimes named on the pricing page against the contact-data add-on.\nprivacy_regimes:\n  - name: GDPR\n    verbatim: 'GDPR and CCPA compliant'\n    source: https://runalphaloops.com/pricing\n  - name: CCPA\n    verbatim: 'GDPR and CCPA compliant'\n    source: https://runalphaloops.com/pricing\n\nsecurity_program:\n  penetration_testing:\n    cadence: weekly\n    provider: Intruder.io\n    methodology: OWASP\n    coverage:\n      - Web applications & APIs\n      - Infrastructure endpoints\n      - OWASP Top 10 vulnerabilities\n      - Emerging threat detection\n    remediation_sla:\n      critical: 7 days\n      high: 14 days\n      medium: 30 days\n      low: 90 days\n  encryption:\n    in_transit: TLS 1.3\n    at_rest: AES-256\n    notes:\n      - Perfect forward secrecy\n      - Encrypted\
  \ database connections\n  authentication:\n    - 100% MFA enforcement across all systems\n    - FIDO2/WebAuthn hardware key support\n    - Phishing-resistant authentication methods\n    - Rate limiting and account lockout protection\n  access_control:\n    - Row-level security (RLS) for data isolation\n    - Least privilege access model\n    - Quarterly access reviews\n    - 24-hour deprovisioning SLA\n  infrastructure:\n    - DDoS protection via Cloudflare\n    - Web Application Firewall (WAF)\n    - Network segmentation\n    - API rate limiting\n  monitoring:\n    - Real-time security event logging\n    - Anomaly detection systems\n    - Automated threat response\n    - Comprehensive audit trails\n  data_minimization: >-\n    \"Only process DOT numbers - no sensitive personal or financial data\" — as published. Note this\n    sits in tension with the product's own contact-enrichment surface, which returns work email,\n    personal emails, phone numbers and employment history for named\
  \ individuals\n    (see openapi EnrichedContact schema and the contact-credits add-on on the pricing page).\n\nevidence:\n  - url: https://runalphaloops.com/security\n    http_status: 200\n    note: Server-rendered; all certification and control claims above read from this page.\n  - url: https://trust.runalphaloops.com/\n    http_status: 200\n    note: Vanta-hosted Trust Center; JS-rendered, no certifications present in served HTML.\n  - url: https://runalphaloops.com/pricing\n    http_status: 200\n    note: GDPR/CCPA claim against the contact-data add-on.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/security/alphaloops-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, NIST Cybersecurity Framework, COBIT
tags:
- fmcsa api
- safer web api
- dot lookup
- carrier data
- Freight
- Trucking
- motor carrier
- fleet intelligence
- Sales Intelligence
- MCP Server
- Contact Enrichment
- Risk
- Fraud
trust_url: https://trust.runalphaloops.com/
---
