---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prompthealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; sp=none; rua=mailto:re+smx8eqvipwe@inbound.dmarcdigests.com; ruf=mailto:dmarcforensics@promptemr.com; fo=0:1:d:s; aspf=r; pct=5
  dnssec: false
  domain: promptemr.com
  note: Legacy/product domain still carrying the application, identity provider, status page and support email. DMARC is enforced at pct=5 with sp=none, so 95% of failing mail is unaffected and subdomains are exempted — weaker in practice than the policy token suggests. No CAA record and no DNSSEC.
  spf: true
  spf_record: v=spf1 include:servers.mcsv.net include:_spf.google.com include:5576817.spf10.hubspotemail.net include:_spf.psm.knowbe4.com include:helpscoutemail.com include:spf.protection.outlook.com -all
hosts:
- cert_expires: Nov 16 18:04:11 2026 GMT
  host: www.prompthealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: authenticate.promptemr.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: OpenID Connect identity provider for the Prompt application.
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: go.promptemr.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  note: Prompt application (SPA). Answers 200 with the same shell for every path.
  tls_version: TLSv1.3
- cert_expires: Oct 11 04:50:46 2026 GMT
  host: status.promptemr.com
  hsts: false
  hsts_max_age: null
  https: true
  note: Atlassian Statuspage — no HSTS header returned.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prompt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prompt, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prompt
provider_slug: prompt
slug: prompt-domain-security
source_filename: prompt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (www.prompthealth.com written by probe-domain-security.py;\n  the promptemr.com application/identity/status hosts added by direct probe in the same pass)\nhosts:\n- host: www.prompthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 18:04:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: authenticate.promptemr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: OpenID Connect identity provider for the Prompt application.\n- host: go.promptemr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n  note: Prompt application (SPA). Answers 200 with the same shell for every path.\n- host: status.promptemr.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Oct 11 04:50:46 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  note: Atlassian Statuspage — no HSTS header returned.\ndomains:\n- domain: prompthealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: promptemr.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:servers.mcsv.net include:_spf.google.com include:5576817.spf10.hubspotemail.net\n    include:_spf.psm.knowbe4.com include:helpscoutemail.com include:spf.protection.outlook.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1; p=quarantine; sp=none; rua=mailto:re+smx8eqvipwe@inbound.dmarcdigests.com; ruf=mailto:dmarcforensics@promptemr.com;\n    fo=0:1:d:s; aspf=r; pct=5\n  note: Legacy/product domain still carrying the application, identity provider, status page and support\n    email. DMARC is enforced at pct=5 with sp=none, so 95% of failing mail is unaffected and subdomains\n    are exempted — weaker in practice\
  \ than the policy token suggests. No CAA record and no DNSSEC.\nfindings:\n- No CAA record on either prompthealth.com or promptemr.com — any public CA may issue for these names.\n- Neither domain is DNSSEC-signed.\n- prompthealth.com publishes DMARC p=reject; promptemr.com publishes p=quarantine with pct=5 and sp=none,\n  which is materially weaker for the domain that actually hosts the application, the identity provider\n  and support@promptemr.com.\n- HSTS is present on www.prompthealth.com, authenticate.promptemr.com and go.promptemr.com; absent on\n  status.promptemr.com.\n- All hosts negotiate TLS 1.3.\nx-evidence:\n  checked: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prompt/refs/heads/main/security/prompt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Electronic Medical Records
- Practice Management
- Physical Therapy
- Rehabilitation Therapy
- Health IT
- Medical Billing
- Patient Engagement
- Artificial Intelligence
---
