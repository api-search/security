---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: immune-onc.com
  mx:
  - smtp.secureserver.net
  - mailstore1.secureserver.net
  note: Public web domain (Squarespace-hosted marketing site). It publishes MX records and therefore accepts mail, but has no SPF TXT record and no _dmarc record, so mail claiming to come from @immune-onc.com has no published sender authentication or reporting policy.
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=100
  dnssec: false
  domain: immuneonc.com
  mx:
  - immuneonc-com.mail.protection.outlook.com
  note: Corporate mail domain (Microsoft 365), published on the company website as the contact address info@immuneonc.com. Distinct from the hyphenated web domain. Added by hand-probe because it is never referenced as a host in apis.yml and so is invisible to the automated host walk.
  spf: true
  spf_record: v=spf1 ip4:50.209.135.157/29 include:spf.protection.outlook.com ~all
  web: 'Its web root resolves and returns 200, but only by redirecting to https://www.immune-onc.com/ — it serves no distinct site. Re-probed 2026-08-04 for /.well-known/security.txt, /.well-known/agent-card.json, /.well-known/agent.json, /llms.txt and /openapi.json: all 404.'
hosts:
- cert_expires: Oct  3 20:57:23 2026 GMT
  host: www.immune-onc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Immune Onc Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Immune-Onc Therapeutics, probed live across 1 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Immune-Onc Therapeutics
provider_slug: immune-onc-therapeutics
slug: immune-onc-therapeutics-domain-security
source_filename: immune-onc-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.immune-onc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:57:23 2026 GMT\n  hsts: null\ndomains:\n- domain: immune-onc.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  mx: [smtp.secureserver.net, mailstore1.secureserver.net]\n  note: >-\n    Public web domain (Squarespace-hosted marketing site). It publishes MX records and therefore\n    accepts mail, but has no SPF TXT record and no _dmarc record, so mail claiming to come from\n    @immune-onc.com has no published sender authentication or reporting policy.\n- domain: immuneonc.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 ip4:50.209.135.157/29 include:spf.protection.outlook.com ~all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; pct=100'\n  mx: [immuneonc-com.mail.protection.outlook.com]\n  web: >-\n   \
  \ Its web root resolves and returns 200, but only by redirecting to https://www.immune-onc.com/ —\n    it serves no distinct site. Re-probed 2026-08-04 for /.well-known/security.txt,\n    /.well-known/agent-card.json, /.well-known/agent.json, /llms.txt and /openapi.json: all 404.\n  note: >-\n    Corporate mail domain (Microsoft 365), published on the company website as the contact address\n    info@immuneonc.com. Distinct from the hyphenated web domain. Added by hand-probe because it is\n    never referenced as a host in apis.yml and so is invisible to the automated host walk.\nprograms:\n  vulnerability_disclosure: none\n  trust_center: none\n  note: >-\n    probe-security-programs.py run 2026-08-04 returned `vdp=none trust=none`. No security.txt\n    Policy/Contact, no bug-bounty program (HackerOne / Bugcrowd / Intigriti), no responsible- or\n    vulnerability-disclosure page, and no trust centre with named certifications (SOC 2, ISO 27001,\n    PCI DSS, HIPAA, FedRAMP) was found on\
  \ any host. Per the pipeline contract no\n    vulnerability-disclosure or trust-center artifact is written and no Security, Compliance or\n    TrustCenter pointer is wired, because there is nothing verified to point at.\nx-evidence:\n  probed: '2026-08-04'\n  method: dig TXT/MX/CAA + _dmarc lookup, TLS/HTTP HEAD\n  findings:\n  - No CAA records on either domain — any public CA may issue for these names.\n  - No DNSSEC on either domain.\n  - No HSTS response header on www.immune-onc.com.\n  - >-\n    The two domains diverge: the mail domain immuneonc.com is SPF- and DMARC-protected\n    (p=quarantine), while the web domain immune-onc.com accepts mail with neither. A look-alike\n    sender on the web domain is the unprotected path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immune-onc-therapeutics/refs/heads/main/security/immune-onc-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Biopharmaceutical
- Oncology
- Immunotherapy
- Immuno-Oncology
- Antibodies
- Clinical Trials
- Life Sciences
- Healthcare
- Drug Development
---
