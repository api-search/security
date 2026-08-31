---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abbott.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: libreview.com
  note: No SPF, DMARC, CAA or DS record published at the apex.
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hellolingo.com
  note: Proofpoint-hosted SPF/DMARC; no CAA, no DNSSEC.
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.abbott.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 09:32:28 2026 GMT
  host: www.libreview.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: Abbott Diabetes Care LibreView platform; serves the only Abbott RFC 9116 security.txt
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.hellolingo.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: Lingo biowearable storefront; serves an llms.txt
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.corelaboratory.abbott
  hsts: false
  https: true
  note: Abbott Core Laboratory; serves an llms.txt. No HSTS header on the root response.
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.cybersecurity.abbott
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  hsts_preload: false
  https: true
  note: 'Abbott product-security site: advisories, CVD program, HDS certification'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abbott Laboratories Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abbott Laboratories, probed live across 5 host(s) and 3 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Abbott Laboratories
provider_slug: abbott-laboratories
slug: abbott-laboratories-domain-security
source_filename: abbott-laboratories-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the Abbott-controlled product hosts found during\n  contract discovery (2026-08-29)\nhosts:\n- host: www.abbott.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.libreview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 09:32:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Abbott Diabetes Care LibreView platform; serves the only Abbott RFC 9116 security.txt\n- host: www.hellolingo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Lingo biowearable storefront; serves an llms.txt\n- host: www.corelaboratory.abbott\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec\
  \ 23 23:59:59 2026 GMT\n  hsts: false\n  note: Abbott Core Laboratory; serves an llms.txt. No HSTS header on the root response.\n- host: www.cybersecurity.abbott\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: false\n  hsts_preload: false\n  note: 'Abbott product-security site: advisories, CVD program, HDS certification'\ndomains:\n- domain: abbott.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: libreview.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: No SPF, DMARC, CAA or DS record published at the apex.\n- domain: hellolingo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: Proofpoint-hosted SPF/DMARC; no CAA, no DNSSEC.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abbott-laboratories/refs/heads/main/security/abbott-laboratories-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Medical Devices
- Diagnostics
- Digital Health
- Life Sciences
- Fortune 500
---
