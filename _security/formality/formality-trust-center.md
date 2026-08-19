---
certifications:
- SOC 2 Type II
- ISO 27001
- GDPR
description: ''
kind: trust-center
layout: security
name: Formality Trust Center
name_suffix: Trust Center
overview: Formality maintains a public trust center documenting SOC 2 Type II, ISO 27001, and GDPR compliance.
provider_name: Formality
provider_slug: formality
slug: formality-trust-center
source_filename: formality-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: true\nsource: https://www.formality.com/en/index.html#security\nurl: https://www.formality.com/en/index.html#security\ncertifications:\n- SOC 2 Type II\n- ISO 27001\n- GDPR\nsecurity_controls_published:\n- {control: access control, detail: 'Granular access control, complete audit trail.'}\n- {control: hosting sovereignty, detail: 'Data stored in Europe or in France (Scaleway).'}\n- {control: AI training exclusion, detail: 'Never trained on your data. Agents operate within a secured perimeter, fully auditable.'}\n- {control: encryption, detail: 'AES-256 at rest, TLS 1.3 in transit.'}\n- {control: reversibility, detail: 'Full export at any time, no lock-in, no opacity.'}\n- {control: SSO enforcement, detail: 'Workspace toggle forcing Google/Microsoft SSO and terminating non-SSO sessions.',\n   source: https://help.formality.com/setup-permissions/user-management}\n- {control: document-access webhook, detail: 'HMAC-SHA256-signed\
  \ notifications on document view, download, bulk download and signature.',\n   source: https://help.formality.com/setup-permissions/user-management}\n- {control: allowed email domains, detail: 'Admins restrict which email domains may be invited.',\n   source: https://help.formality.com/setup-permissions/user-management}\n- {control: audit trail, detail: 'Audit trail plus per-object change history; deactivated users retain history.',\n   source: https://help.formality.com/setup-permissions/changes-audit-trail}\ncommitments:\n- {name: One Clause, detail: 'Signatory of One Clause.'}\ntrust_portal:\n  exists: false\n  subdomain_probed: [trust.formality.com, security.formality.com]\n  note: >-\n    No dedicated trust portal and no automated evidence-sharing centre. Certification\n    claims are prose on the marketing site; no certificate numbers, auditor names,\n    audit scope, report dates or NDA-gated report request flow are published, and the\n    SOC 2 report is not obtainable from any\
  \ public surface.\nurl_correction:\n  previous_url: https://www.formality.com/en/security\n  previous_status: 403\n  checked: '2026-08-17'\n  note: >-\n    DEFECT FIXED THIS ROUND. The 2026-07-19 pass recorded\n    https://www.formality.com/en/security as the source, and both the Compliance and\n    TrustCenter pointers in apis.yml targeted it. That URL now returns HTTP 403 from the\n    S3/CloudFront origin — the standalone security page no longer exists after the site\n    was rebuilt on Framer, and the same is true of the old PrivacyPolicy pointer\n    (/policies/personal-data-protection-policy/, also 403). The certification and\n    security content now lives in the \"Security & sovereignty\" section anchored at\n    /en/index.html#security. apis.yml pointers were repointed accordingly.\nnotes: >-\n  Formality publishes a substantive security posture for a company of its size —\n  ISO 27001 and SOC 2 Type II claimed and renewed annually, EU/France data residency\n  with a named infrastructure\
  \ partner (Scaleway), AES-256 at rest, TLS 1.3 in transit,\n  contractual prohibition on AI vendors training on customer data, full export\n  reversibility, and real tenant-level controls (enforced SSO, email-domain\n  allowlisting, HMAC-signed document-access webhooks, audit trail).\n\n  The weakness is verifiability rather than substance: everything is self-declared prose\n  with no trust portal, no certificate identifiers and no path to the underlying\n  reports. Live probing also surfaced a regression the marketing copy does not mention —\n  the www origin now serves NO HSTS header, and the registrable domain still has no\n  DNSSEC, no CAA records and DMARC at p=none. Those are recorded in\n  security/formality-domain-security.yml.\nevidence:\n- source: https://www.formality.com/en/index.html\n  http_status: 200\n  fetched: '2026-08-17'\n  keywords: [iso 27001, soc 2 type ii, aes-256, tls 1.3, scaleway, one clause, audit trail]\n- source: https://www.formality.com/en/security\n  http_status:\
  \ 403\n  fetched: '2026-08-17'\n  note: previous round's source URL, now dead\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formality/refs/heads/main/security/formality-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, GDPR
tags:
- Company
- Ai/Ml
- Legal
- Contract Management
- Document Management
- Asset Intelligence
- Compliance
- SaaS
trust_url: https://www.formality.com/en/index.html#security
---
