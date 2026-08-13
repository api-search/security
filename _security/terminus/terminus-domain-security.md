---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: demandscience.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: terminus.com
  spf: true
- apex_a_record: false
  caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lastbounce.com
  note: Verify API domain. The apex has NO A record — only NS (Route 53) and mail records — so lastbounce.com itself does not serve a site; the product lives at api/sqa-api/dev-api subdomains and is marketed under the DemandScience brand. No DNSSEC, no CAA. DMARC policy is quarantine with sp=none, weaker than the reject policy on demandscience.com and terminus.com. Probed by hand 2026-08-12.
  spf: true
hosts:
- cert_expires: Sep 14 08:52:20 2026 GMT
  host: demandscience.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 15:22:07 2026 GMT
  host: developer.terminus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: api.terminusplatform.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.lastbounce.com
  hsts: false
  https: true
  note: 'Verify API production host. Added by hand on 2026-08-12: this host was found during contract discovery and is not reached by probe-domain-security.py, which walks only the first apis.yml hosts. Probed directly with openssl s_client and curl.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terminus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terminus, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Terminus
provider_slug: terminus
slug: terminus-domain-security
source_filename: terminus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: demandscience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:52:20 2026 GMT\n  hsts: false\n- host: developer.terminus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:22:07 2026 GMT\n  hsts: false\n- host: api.terminusplatform.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\n- host: api.lastbounce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\n  note: >-\n    Verify API production host. Added by hand on 2026-08-12: this host was found\n    during contract discovery and is not reached by probe-domain-security.py, which\n    walks only the first apis.yml hosts. Probed directly with openssl s_client and\n    curl.\ndomains:\n- domain: demandscience.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n- domain: terminus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lastbounce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  apex_a_record: false\n  note: >-\n    Verify API domain. The apex has NO A record — only NS (Route 53) and mail\n    records — so lastbounce.com itself does not serve a site; the product lives at\n    api/sqa-api/dev-api subdomains and is marketed under the DemandScience brand.\n    No DNSSEC, no CAA. DMARC policy is quarantine with sp=none, weaker than the\n    reject policy on demandscience.com and terminus.com. Probed by hand 2026-08-12.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminus/refs/heads/main/security/terminus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Account Based Marketing
- Marketing
- Advertising
- Sales
- B2B
- Analytics
- Email
- Email Verification
- Data Quality
---
