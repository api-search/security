---
certifications:
- HIPAA
- CLIA
- CAP
description: Nucleus Genomics operates a Vanta-hosted trust center on its own subdomain, trust.mynucleus.com. The page returns HTTP 200 with title "Nucleus Trust Center" and rel=canonical https://trust.mynucleus.com. The document list itself is rendered client-side by the Vanta application and the underlying Vanta trust API returns 401 to anonymous callers, so the individual report artifacts (and whether they require an NDA) could not be read without authentication. The certifications recorded below are the ones Nucleus names in its own prose on mynucleus.com, not values scraped from the trust center UI.
kind: trust-center
layout: security
name: Nucleus Genomics Trust Center
name_suffix: Trust Center
overview: Nucleus Genomics maintains a public trust center documenting HIPAA, CLIA, and CAP compliance.
provider_name: Nucleus Genomics
provider_slug: nucleus-genomics
slug: nucleus-genomics-trust-center
source_filename: nucleus-genomics-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://trust.mynucleus.com/\nname: Nucleus Trust Center\ndescription: Nucleus Genomics operates a Vanta-hosted trust center on its own subdomain,\n  trust.mynucleus.com. The page returns HTTP 200 with title \"Nucleus Trust Center\"\n  and rel=canonical https://trust.mynucleus.com. The document list itself is rendered\n  client-side by the Vanta application and the underlying Vanta trust API returns 401\n  to anonymous callers, so the individual report artifacts (and whether they require\n  an NDA) could not be read without authentication. The certifications recorded below\n  are the ones Nucleus names in its own prose on mynucleus.com, not values scraped from\n  the trust center UI.\nurl: https://trust.mynucleus.com\nplatform: Vanta\nplatform_evidence: page shell loads assets.vanta.com and carries data-slugid it4bbj97jggcpwgm5wh8u\ncertifications:\n- name: HIPAA\n  kind: compliance program\n  claimed_by: provider\n  evidence:\
  \ https://mynucleus.com/privacy-and-security\n- name: CLIA\n  kind: clinical laboratory certification\n  claimed_by: provider\n  evidence: https://mynucleus.com/privacy-and-security\n- name: CAP\n  kind: laboratory accreditation\n  claimed_by: provider\n  evidence: https://mynucleus.com/privacy-and-security\nnot_claimed:\n- SOC 2\n- ISO 27001\n- HITRUST\n- PCI DSS\n- FedRAMP\nsecurity_contact: mailto:security@mynucleus.com\nx-evidence:\n- url: https://trust.mynucleus.com/\n  http_status: 200\n  content_type: text/html\n- url: https://mynucleus.com/privacy-and-security\n  http_status: 200\n- url: https://api.vanta.com/v1/trust-center/it4bbj97jggcpwgm5wh8u\n  http_status: 401\n  note: anonymous trust-center data API is gated\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nucleus-genomics/refs/heads/main/security/nucleus-genomics-trust-center.yml
summary_line: HIPAA, CLIA, CAP
tags:
- Company
- Genomics
- Health
- Consumer Genetics
- Whole Genome Sequencing
- Fertility
- IVF
- Carrier Screening
- Precision Medicine
- Biotechnology
trust_url: https://trust.mynucleus.com
---
